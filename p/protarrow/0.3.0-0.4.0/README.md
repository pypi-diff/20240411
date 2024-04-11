# Comparing `tmp/protarrow-0.3.0.tar.gz` & `tmp/protarrow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.3.0.tar", max compression
+gzip compressed data, was "protarrow-0.4.0.tar", max compression
```

## Comparing `protarrow-0.3.0.tar` & `protarrow-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    10140 2024-03-25 11:45:54.901895 protarrow-0.3.0/LICENSE
--rw-r--r--   0        0        0       95 2024-03-25 11:45:54.901895 protarrow-0.3.0/NOTICE
--rw-r--r--   0        0        0     3022 2024-03-25 11:45:54.901895 protarrow-0.3.0/README.md
--rw-r--r--   0        0        0      754 2024-03-25 11:46:09.945941 protarrow-0.3.0/protarrow/__init__.py
--rw-r--r--   0        0        0    20762 2024-03-25 11:45:54.905895 protarrow-0.3.0/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7884 2024-03-25 11:45:54.905895 protarrow-0.3.0/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1564 2024-03-25 11:45:54.905895 protarrow-0.3.0/protarrow/common.py
--rw-r--r--   0        0        0     4621 2024-03-25 11:45:54.905895 protarrow-0.3.0/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18482 2024-03-25 11:45:54.905895 protarrow-0.3.0/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0      872 2024-03-25 11:45:54.905895 protarrow-0.3.0/protarrow/test_arrow_to_proto.py
--rw-r--r--   0        0        0     1979 2024-03-25 11:46:09.945941 protarrow-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10140 2024-04-11 12:53:22.158708 protarrow-0.4.0/LICENSE
+-rw-r--r--   0        0        0       95 2024-04-11 12:53:22.158708 protarrow-0.4.0/NOTICE
+-rw-r--r--   0        0        0     3022 2024-04-11 12:53:22.158708 protarrow-0.4.0/README.md
+-rw-r--r--   0        0        0      754 2024-04-11 12:53:40.562839 protarrow-0.4.0/protarrow/__init__.py
+-rw-r--r--   0        0        0    20762 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7813 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1564 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18323 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1979 2024-04-11 12:53:40.562839 protarrow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.4.0/PKG-INFO
```

### Comparing `protarrow-0.3.0/LICENSE` & `protarrow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.3.0/README.md` & `protarrow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `protarrow-0.3.0/protarrow/__init__.py` & `protarrow-0.4.0/protarrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.3.0/protarrow/arrow_to_proto.py` & `protarrow-0.4.0/protarrow/arrow_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.3.0/protarrow/cast_to_proto.py` & `protarrow-0.4.0/protarrow/cast_to_proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 assert results.type == config.enum_type
             else:
                 results = array.cast(config.enum_type)
         else:
             results = array.cast(
                 _PROTO_PRIMITIVE_TYPE_TO_PYARROW[field_descriptor.type]
             )
-        if results.null_count > 0:
+        if not field_descriptor.has_presence and results.null_count > 0:
             return results.fill_null(get_arrow_default_value(field_descriptor, config))
         else:
             return results
 
 
 def _cast_array(
     array: pa.Array,
@@ -126,18 +126,15 @@
     source_array: Optional[pa.Array],
     num_rows: int,
     config: ProtarrowConfig,
 ) -> Tuple[pa.Array, pa.Field]:
     expected_field = field_descriptor_to_field(field_descriptor, config)
     if source_array is not None:
         casted_array = _cast_array(source_array, field_descriptor, config)
-    elif (
-        field_descriptor.type == FieldDescriptor.TYPE_MESSAGE
-        and field_descriptor.label != FieldDescriptor.LABEL_REPEATED
-    ):
+    elif field_descriptor.has_presence:
         casted_array = pa.nulls(num_rows, expected_field.type)
         if pa.types.is_struct(expected_field.type):
             casted_array = cast_struct_array(
                 casted_array, field_descriptor.message_type, config
             )
     else:
         default_value = (
```

### Comparing `protarrow-0.3.0/protarrow/common.py` & `protarrow-0.4.0/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.3.0/protarrow/message_extractor.py` & `protarrow-0.4.0/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.3.0/protarrow/proto_to_arrow.py` & `protarrow-0.4.0/protarrow/proto_to_arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
             ),
             nullable=config.list_nullable,
         )
     else:
         return pa.field(
             field_descriptor.name,
             field_descriptor_to_data_type(field_descriptor, config),
-            nullable=field_descriptor.type == FieldDescriptor.TYPE_MESSAGE,
+            nullable=field_descriptor.has_presence,
         )
 
 
 def field_descriptor_to_data_type(
     field_descriptor: FieldDescriptor,
     config: ProtarrowConfig,
 ) -> pa.DataType:
@@ -342,15 +342,15 @@
     converter = _get_converter(field_descriptor, config)
 
     if converter is not None:
         data_type = field_descriptor_to_data_type(field_descriptor, config)
         null_value = (
             None
             if (
-                field_descriptor.type == FieldDescriptor.TYPE_MESSAGE
+                field_descriptor.has_presence
                 # We use none for repeated field as there should not
                 # be any missing list elements, they are not nullable
                 or field_descriptor.label == FieldDescriptor.LABEL_REPEATED
             )
             else converter(field_descriptor.default_value)
         )
         array = []
@@ -447,24 +447,21 @@
     field_descriptor: FieldDescriptor, config: ProtarrowConfig
 ) -> bool:
     if is_map(field_descriptor):
         return config.map_nullable
     elif field_descriptor.label == FieldDescriptorProto.LABEL_REPEATED:
         return config.list_nullable
     else:
-        return field_descriptor.type == FieldDescriptorProto.TYPE_MESSAGE
+        return field_descriptor.has_presence
 
 
 def _proto_field_validity_mask(
     messages: Iterable[Message], field_descriptor: FieldDescriptor
 ) -> Optional[List[bool]]:
-    if (
-        field_descriptor.type != FieldDescriptorProto.TYPE_MESSAGE
-        or field_descriptor.label == FieldDescriptorProto.LABEL_REPEATED
-    ):
+    if not field_descriptor.has_presence:
         return None
     mask = []
     field_name = field_descriptor.name
     for record in messages:
         if record is None:
             mask.append(False)
         else:
@@ -511,17 +508,19 @@
                 nullable=_proto_field_nullable(field_descriptor, config),
             )
         )
 
     return pa.StructArray.from_arrays(
         arrays=arrays,
         fields=fields,
-        mask=pc.invert(pa.array(validity_mask, pa.bool_()))
-        if validity_mask is not None
-        else pa.repeat(False, len(messages)),
+        mask=(
+            pc.invert(pa.array(validity_mask, pa.bool_()))
+            if validity_mask is not None
+            else pa.repeat(False, len(messages))
+        ),
     )
 
 
 def messages_to_record_batch(
     messages: Iterable[M],
     message_type: Type[M],
     config: ProtarrowConfig = ProtarrowConfig(),
```

### Comparing `protarrow-0.3.0/pyproject.toml` & `protarrow-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.3.0"
+version = "0.4.0"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
```

### Comparing `protarrow-0.3.0/PKG-INFO` & `protarrow-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.3.0
+Version: 0.4.0
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
```

