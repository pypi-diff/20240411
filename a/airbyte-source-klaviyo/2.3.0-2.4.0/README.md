# Comparing `tmp/airbyte_source_klaviyo-2.3.0.tar.gz` & `tmp/airbyte_source_klaviyo-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_klaviyo-2.3.0.tar", max compression
+gzip compressed data, was "airbyte_source_klaviyo-2.4.0.tar", max compression
```

## Comparing `airbyte_source_klaviyo-2.3.0.tar` & `airbyte_source_klaviyo-2.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4514 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/README.md
--rw-r--r--   0        0        0      746 2024-03-21 02:10:36.845538 airbyte_source_klaviyo-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/__init__.py
--rw-r--r--   0        0        0      975 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/availability_strategy.py
--rw-r--r--   0        0        0      196 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/exceptions.py
--rw-r--r--   0        0        0      233 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/run.py
--rw-r--r--   0        0        0     4429 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/campaigns.json
--rw-r--r--   0        0        0      935 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/email_templates.json
--rw-r--r--   0        0        0     2136 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/events.json
--rw-r--r--   0        0        0     2262 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/flows.json
--rw-r--r--   0        0        0     3931 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/global_exclusions.json
--rw-r--r--   0        0        0     1839 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/lists.json
--rw-r--r--   0        0        0      787 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/metrics.json
--rw-r--r--   0        0        0     3931 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/profiles.json
--rw-r--r--   0        0        0     2892 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/shared/subscriptions.json
--rw-r--r--   0        0        0     2851 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/source.py
--rw-r--r--   0        0        0     1114 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/spec.json
--rw-r--r--   0        0        0    14710 2024-03-21 01:47:20.529994 airbyte_source_klaviyo-2.3.0/source_klaviyo/streams.py
--rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4514 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/README.md
+-rw-r--r--   0        0        0      746 2024-04-11 15:18:13.871414 airbyte_source_klaviyo-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/availability_strategy.py
+-rw-r--r--   0        0        0      196 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/exceptions.py
+-rw-r--r--   0        0        0      233 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/run.py
+-rw-r--r--   0        0        0     4491 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/campaigns.json
+-rw-r--r--   0        0        0      935 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/email_templates.json
+-rw-r--r--   0        0        0     2136 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/events.json
+-rw-r--r--   0        0        0     2262 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/flows.json
+-rw-r--r--   0        0        0     3931 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/global_exclusions.json
+-rw-r--r--   0        0        0     1839 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/lists.json
+-rw-r--r--   0        0        0      787 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/metrics.json
+-rw-r--r--   0        0        0     3931 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/profiles.json
+-rw-r--r--   0        0        0     2892 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/shared/subscriptions.json
+-rw-r--r--   0        0        0     2851 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/source.py
+-rw-r--r--   0        0        0     1114 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/spec.json
+-rw-r--r--   0        0        0    14710 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/streams.py
+-rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.4.0/PKG-INFO
```

### Comparing `airbyte_source_klaviyo-2.3.0/README.md` & `airbyte_source_klaviyo-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/pyproject.toml` & `airbyte_source_klaviyo-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.3.0"
+version = "2.4.0"
 name = "airbyte-source-klaviyo"
 description = "Source implementation for Klaviyo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/availability_strategy.py` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/campaigns.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/campaigns.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999599358974358%*

 * *Differences: {"'properties'": "{'attributes': {'properties': {'audiences': {'properties': "*

 * *                 "OrderedDict([('included', OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'string'])]))])), ('excluded', "*

 * *                 "OrderedDict([('type', ['null', 'array']), ('items', OrderedDict([('type', "*

 * *                 "['null', 'string'])]))]))]), delete: ['included', 'excluded']}}}}"}*

```diff
@@ -6,37 +6,39 @@
             "additionalProperties": true,
             "properties": {
                 "archived": {
                     "type": "boolean"
                 },
                 "audiences": {
                     "additionalProperties": true,
-                    "excluded": {
-                        "items": {
+                    "properties": {
+                        "excluded": {
+                            "items": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
                             "type": [
                                 "null",
-                                "string"
+                                "array"
                             ]
                         },
-                        "type": [
-                            "null",
-                            "array"
-                        ]
-                    },
-                    "included": {
-                        "items": {
+                        "included": {
+                            "items": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
                             "type": [
                                 "null",
-                                "string"
+                                "array"
                             ]
-                        },
-                        "type": [
-                            "null",
-                            "array"
-                        ]
+                        }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
                 "channel": {
```

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/email_templates.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/email_templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/events.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/flows.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/flows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/global_exclusions.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/global_exclusions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/lists.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/metrics.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/profiles.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/profiles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/schemas/shared/subscriptions.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/shared/subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/source.py` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/spec.json` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/source_klaviyo/streams.py` & `airbyte_source_klaviyo-2.4.0/source_klaviyo/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.3.0/PKG-INFO` & `airbyte_source_klaviyo-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-klaviyo
-Version: 2.3.0
+Version: 2.4.0
 Summary: Source implementation for Klaviyo.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

