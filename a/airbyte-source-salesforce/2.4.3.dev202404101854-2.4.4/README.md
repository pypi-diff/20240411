# Comparing `tmp/airbyte_source_salesforce-2.4.3.dev202404101854.tar.gz` & `tmp/airbyte_source_salesforce-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.4.3.dev202404101854.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.4.4.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.4.3.dev202404101854.tar` & `airbyte_source_salesforce-2.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/README.md
--rw-r--r--   0        0        0      842 2024-04-10 18:54:32.199071 airbyte_source_salesforce-2.4.3.dev202404101854/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/__init__.py
--rw-r--r--   0        0        0    16870 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/api.py
--rw-r--r--   0        0        0     1667 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     3946 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/run.py
--rw-r--r--   0        0        0     9747 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    14130 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    41238 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-04-10 18:52:01.301816 airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/utils.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.3.dev202404101854/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/README.md
+-rw-r--r--   0        0        0      826 2024-04-09 20:25:39.281002 airbyte_source_salesforce-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    16870 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/api.py
+-rw-r--r--   0        0        0     1667 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3946 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/run.py
+-rw-r--r--   0        0        0     9747 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    14130 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    41238 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.4/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/README.md` & `airbyte_source_salesforce-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/pyproject.toml` & `airbyte_source_salesforce-2.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.4.3.dev202404101854"
+version = "2.4.4"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/api.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/run.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/schemas/Describe.json` & `airbyte_source_salesforce-2.4.4/source_salesforce/schemas/Describe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/source.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.4.4/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/streams.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/source_salesforce/utils.py` & `airbyte_source_salesforce-2.4.4/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.3.dev202404101854/PKG-INFO` & `airbyte_source_salesforce-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.4.3.dev202404101854
+Version: 2.4.4
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

