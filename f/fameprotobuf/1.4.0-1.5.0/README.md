# Comparing `tmp/fameprotobuf-1.4.0.tar.gz` & `tmp/fameprotobuf-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fameprotobuf-1.4.0.tar", max compression
+gzip compressed data, was "fameprotobuf-1.5.0.tar", max compression
```

## Comparing `fameprotobuf-1.4.0.tar` & `fameprotobuf-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2938 2024-03-17 15:26:17.737351 fameprotobuf-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    10389 2021-05-27 13:16:26.709773 fameprotobuf-1.4.0/LICENSE
-drwxr-xr-x   0        0        0        0 2024-03-17 15:26:17.738350 fameprotobuf-1.4.0/LICENSES/
--rw-r--r--   0        0        0     1182 2024-03-17 15:26:17.741351 fameprotobuf-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2258 2024-03-17 15:26:17.739353 fameprotobuf-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-03-17 15:51:40.898088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/__init__.py
--rw-r--r--   0        0        0     3983 2024-03-17 15:51:40.890088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/AgentMessage_pb2.py
--rw-r--r--   0        0        0     3854 2024-03-17 15:51:40.890088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/AgentMessage_pb2.pyi
--rw-r--r--   0        0        0     2076 2024-03-17 15:51:40.891088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Bundle_pb2.py
--rw-r--r--   0        0        0     2057 2024-03-17 15:51:40.891088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Bundle_pb2.pyi
--rw-r--r--   0        0        0     1729 2024-03-17 15:51:40.892089 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Contract_pb2.py
--rw-r--r--   0        0        0     1571 2024-03-17 15:51:40.892089 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Contract_pb2.pyi
--rw-r--r--   0        0        0     1781 2024-03-17 15:51:40.893089 fameprotobuf-1.4.0/src/main/python/fameprotobuf/DataStorage_pb2.py
--rw-r--r--   0        0        0     1210 2024-03-17 15:51:40.893089 fameprotobuf-1.4.0/src/main/python/fameprotobuf/DataStorage_pb2.pyi
--rw-r--r--   0        0        0     2356 2024-03-17 15:51:40.894088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/ExecutionData_pb2.py
--rw-r--r--   0        0        0     2551 2024-03-17 15:51:40.894088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/ExecutionData_pb2.pyi
--rw-r--r--   0        0        0     1538 2024-03-17 15:51:40.895087 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Field_pb2.py
--rw-r--r--   0        0        0     1588 2024-03-17 15:51:40.895087 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Field_pb2.pyi
--rw-r--r--   0        0        0     3178 2024-03-17 15:51:40.896088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/InputFile_pb2.py
--rw-r--r--   0        0        0     4238 2024-03-17 15:51:40.896088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/InputFile_pb2.pyi
--rw-r--r--   0        0        0     1221 2024-03-17 15:51:40.897088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Model_pb2.py
--rw-r--r--   0        0        0      496 2024-03-17 15:51:40.897088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Model_pb2.pyi
--rw-r--r--   0        0        0     4012 2024-03-17 15:51:40.897088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Services_pb2.py
--rw-r--r--   0        0        0     5708 2024-03-17 15:51:40.898088 fameprotobuf-1.4.0/src/main/python/fameprotobuf/Services_pb2.pyi
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 fameprotobuf-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3098 2024-04-11 08:50:40.870601 fameprotobuf-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10389 2021-05-27 13:16:26.709773 fameprotobuf-1.5.0/LICENSE
+drwxr-xr-x   0        0        0        0 2024-03-17 15:26:17.738350 fameprotobuf-1.5.0/LICENSES/
+-rw-r--r--   0        0        0     1081 2024-04-11 09:02:20.760000 fameprotobuf-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2258 2024-03-17 15:26:17.739353 fameprotobuf-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 09:02:20.768883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/__init__.py
+-rw-r--r--   0        0        0     3983 2024-04-11 09:02:20.761867 fameprotobuf-1.5.0/src/main/python/fameprotobuf/AgentMessage_pb2.py
+-rw-r--r--   0        0        0     3854 2024-04-11 09:02:20.761867 fameprotobuf-1.5.0/src/main/python/fameprotobuf/AgentMessage_pb2.pyi
+-rw-r--r--   0        0        0     2076 2024-04-11 09:02:20.762883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Bundle_pb2.py
+-rw-r--r--   0        0        0     2057 2024-04-11 09:02:20.762883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Bundle_pb2.pyi
+-rw-r--r--   0        0        0     1729 2024-04-11 09:02:20.762883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Contract_pb2.py
+-rw-r--r--   0        0        0     1571 2024-04-11 09:02:20.763882 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Contract_pb2.pyi
+-rw-r--r--   0        0        0     1781 2024-04-11 09:02:20.763882 fameprotobuf-1.5.0/src/main/python/fameprotobuf/DataStorage_pb2.py
+-rw-r--r--   0        0        0     1210 2024-04-11 09:02:20.764883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/DataStorage_pb2.pyi
+-rw-r--r--   0        0        0     2356 2024-04-11 09:02:20.764883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/ExecutionData_pb2.py
+-rw-r--r--   0        0        0     2551 2024-04-11 09:02:20.764883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/ExecutionData_pb2.pyi
+-rw-r--r--   0        0        0     1538 2024-04-11 09:02:20.765883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Field_pb2.py
+-rw-r--r--   0        0        0     1588 2024-04-11 09:02:20.765883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Field_pb2.pyi
+-rw-r--r--   0        0        0     3178 2024-04-11 09:02:20.766883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/InputFile_pb2.py
+-rw-r--r--   0        0        0     4238 2024-04-11 09:02:20.766883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/InputFile_pb2.pyi
+-rw-r--r--   0        0        0     1567 2024-04-11 09:02:20.766883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Model_pb2.py
+-rw-r--r--   0        0        0     1378 2024-04-11 09:02:20.767883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Model_pb2.pyi
+-rw-r--r--   0        0        0     4012 2024-04-11 09:02:20.767883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Services_pb2.py
+-rw-r--r--   0        0        0     5708 2024-04-11 09:02:20.768883 fameprotobuf-1.5.0/src/main/python/fameprotobuf/Services_pb2.pyi
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 fameprotobuf-1.5.0/PKG-INFO
```

### Comparing `fameprotobuf-1.4.0/CHANGELOG.md` & `fameprotobuf-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 <!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: CC0-1.0 -->
 # Changelog
 
-## [1.4.0 - 2024-03-17](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.4.0)
+## [1.5.0](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.5.0) - 2024-04-11
+### Added
+- Add java package section to Model #43 (@dlr-cjs)
+
+## [1.4.0](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.4.0) - 2024-03-17
 ### Changed
-- Use 2-space indentation in all .proto files #20 (dlr-cjs)
+- Use 2-space indentation in all .proto files #20 (@dlr-cjs)
 
 ### Added
-- Add new optional section to DataStorage holding simulation execution details #21 (dlr-cjs)
-- Add new optional section to DataStorage holding model details #20 (dlr-cjs)
-- Add new optional entry to NestedField telling whether a field is of type "list" #34 (dlr-cjs)
-- Add license string to each .proto file #35 (dlr-cjs)
-- Ensure reuse compatibility in CI #35 (dlr-cjs)
-- Ensure CHANGELOG is up to date in CI #36 (dlr-cjs)
+- Add new optional section to DataStorage holding simulation execution details #21 (@dlr-cjs)
+- Add new optional section to DataStorage holding model details #20 (@dlr-cjs)
+- Add new optional entry to NestedField telling whether a field is of type "list" #34 (@dlr-cjs)
+- Add license string to each .proto file #35 (@dlr-cjs)
+- Ensure reuse compatibility in CI #35 (@dlr-cjs)
+- Ensure CHANGELOG is up to date in CI #36 (@dlr-cjs)
 
-## [1.3.1 - 2023-11-29](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.3.1)
+## [1.3.1](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.3.1) - 2023-11-29
 ### Changed
 - Loosen maximum supported Python version #33 (@dlr-cjs @dlr_fn)
 
-## [1.3.0 - 2023-11-22](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.3.0)
+## [1.3.0](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.3.0) - 2023-11-22
 ### Changed 
 - Switch to pyproject.toml to replace setup.py #32 (@dlr-cjs)
 - Reformat Changelog to follow style guide #29 (@dlr-cjs)
 - Update to latest protobuf version 24 #31 (@dlr-cjs)
 - Update README.md #32 (@dlr-cjs, @dlr_fn)
 
 ### Added
 - Provide Python interface files (#30 @dlr-cjs)
 
-## [1.2.1 - 2023-05-03](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.2.1)
+## [1.2.1](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.2.1) - 2023-05-03
 ### Changed
 - Remove `ProgramParam` from InputData - regarded as non-breaking as it was not used so far
 
 ### Added
 - Store a schema in InputData
 - Add optional MetaData field to AgentDao 
 - Add optional MetaData field to ProtoContract 
 - Update to latest protobuf version 22
 
-## [1.2 - 2022-07-08](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.2)
+## [1.2](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.2) - 2022-07-08
 ### Changed
 - Output messages may now contain multiple key-value mappings per column
 - Update to latest protobuf version 21
 
-## [1.1.5 - 2021-06-10](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.5)
+## [1.1.5](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.5) - 2021-06-10
 ### Changed
 - Extract version number from `pom.xml` in setup.py
 - Ensure that files are compiled before committing to PyPI
 
-## [1.1.4 - 2021-0607](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.4)
+## [1.1.4](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.4) - 2021-0607
 ### Added
 - Add missing setup.yaml parameters
 - Add long values for Fields
 
 ### Changed
 - Make long, int, and string repeatable for Fields
 
 ### Removed
 - Remove default values of Fields
 
 ## 1.1.3 - Retracted
 
-## [1.1.2 - 2021-0311](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.2)
+## [1.1.2](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.2) - 2021-0311
 ### Changed
 - Update Contracts to feature recursive fields
 
-## [1.1.1 - 2021-02-19](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.1)
+## [1.1.1](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.1) - 2021-02-19
 ### Changed
 - Restructure Inputs to allow nested Fields  
 
-## [1.1.0 - 2021-02-11](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.0)
+## [1.1.0](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.1.0) - 2021-02-11
 ### Changed
 - Automate packaging to PyPI
 
-## [1.0 - 2021-02-09](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.0)
+## [1.0](https://gitlab.com/fame-framework/fame-protobuf/-/tags/v1.0) - 2021-02-09
 _Initial release._
```

### Comparing `fameprotobuf-1.4.0/LICENSE` & `fameprotobuf-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/pyproject.toml` & `fameprotobuf-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
-# 
-# SPDX-License-Identifier: Apache-2.0
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fameprotobuf"
-version = "1.4.0"
+version = "1.5.0"
 description = "Protobuf definitions converted to python classes for use in `fameio`"
 license = "Apache-2.0"
 authors = [ "Christoph Schimeczek <fame@dlr.de>", "Ulrich Frey <fame@dlr.de>", "Marc Deissenroth-Uhrig <fame@dlr.de>", "Benjamin Fuchs <fame@dlr.de>", "Felix Nitsch <fame@dlr.de>",]
 maintainers = [ "Christoph Schimeczek <fame@dlr.de>",]
 readme = "README.md"
 homepage = "https://gitlab.com/fame-framework/wiki/-/wikis/home"
 repository = "https://gitlab.com/fame-framework/fame-protobuf"
 keywords = [ "protobuffer", "FAME", "framework", "fameio", "agent-based modelling",]
 classifiers = [ "Development Status :: 5 - Production/Stable", "Operating System :: OS Independent", "Topic :: Scientific/Engineering",]
-include = [ "CHANGELOG.md", "src/main/python/**/*"]
-packages = [{include = "fameprotobuf", from = "src/main/python"}]
+include = [ "CHANGELOG.md", "src/main/python/**/*",]
+[[tool.poetry.packages]]
+include = "fameprotobuf"
+from = "src/main/python"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-protobuf = "^4.21.1"
+protobuf = "^4.21.1"
```

### Comparing `fameprotobuf-1.4.0/README.md` & `fameprotobuf-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/AgentMessage_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/AgentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/AgentMessage_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/AgentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Bundle_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Bundle_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Contract_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Contract_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Contract_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Contract_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/DataStorage_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/DataStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/DataStorage_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/DataStorage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/ExecutionData_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/ExecutionData_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/ExecutionData_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/ExecutionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Field_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Field_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Field_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Field_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/InputFile_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/InputFile_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/InputFile_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/InputFile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Model_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Model_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bModel.proto\x12\x05model\"*\n\tModelData\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\tB$\n\x1b\x64\x65.dlr.gitlab.fame.protobufB\x05Model')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bModel.proto\x12\x05model\"\x9e\x01\n\tModelData\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x08packages\x18\x03 \x01(\x0b\x32\x1d.model.ModelData.JavaPackages\x1a\x41\n\x0cJavaPackages\x12\r\n\x05\x61gent\x18\x01 \x03(\t\x12\x10\n\x08\x64\x61taItem\x18\x02 \x03(\t\x12\x10\n\x08portable\x18\x03 \x03(\tB$\n\x1b\x64\x65.dlr.gitlab.fame.protobufB\x05Model')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'Model_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\033de.dlr.gitlab.fame.protobufB\005Model'
-  _globals['_MODELDATA']._serialized_start=22
-  _globals['_MODELDATA']._serialized_end=64
+  _globals['_MODELDATA']._serialized_start=23
+  _globals['_MODELDATA']._serialized_end=181
+  _globals['_MODELDATA_JAVAPACKAGES']._serialized_start=116
+  _globals['_MODELDATA_JAVAPACKAGES']._serialized_end=181
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Services_pb2.py` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Services_pb2.py`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/src/main/python/fameprotobuf/Services_pb2.pyi` & `fameprotobuf-1.5.0/src/main/python/fameprotobuf/Services_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fameprotobuf-1.4.0/PKG-INFO` & `fameprotobuf-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fameprotobuf
-Version: 1.4.0
+Version: 1.5.0
 Summary: Protobuf definitions converted to python classes for use in `fameio`
 Home-page: https://gitlab.com/fame-framework/wiki/-/wikis/home
 License: Apache-2.0
 Keywords: protobuffer,FAME,framework,fameio,agent-based modelling
 Author: Christoph Schimeczek
 Author-email: fame@dlr.de
 Maintainer: Christoph Schimeczek
```

