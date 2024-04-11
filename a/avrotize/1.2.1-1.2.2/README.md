# Comparing `tmp/avrotize-1.2.1.tar.gz` & `tmp/avrotize-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.2.1.tar` & `avrotize-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    25773 2024-04-09 15:03:53.116738 avrotize-1.2.1/README.md
--rw-r--r--   0        0        0     1321 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-09 15:03:57.848686 avrotize-1.2.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15558 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    11455 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    13646 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    11615 2024-04-09 15:03:53.116738 avrotize-1.2.1/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18100 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    12056 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotopython.py
--rw-r--r--   0        0        0     9593 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91241 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15532 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-09 15:03:53.120738 avrotize-1.2.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-09 15:03:53.120738 avrotize-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    26440 1970-01-01 00:00:00.000000 avrotize-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    25996 2024-04-11 14:43:14.781846 avrotize-1.2.2/README.md
+-rw-r--r--   0        0        0     1673 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-11 14:43:19.905905 avrotize-1.2.2/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15558 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotize.py
+-rw-r--r--   0        0        0    31485 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    18518 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12102 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18100 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13086 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10151 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91408 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-11 14:43:14.785846 avrotize-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    26663 1970-01-01 00:00:00.000000 avrotize-1.2.2/PKG-INFO
```

### Comparing `avrotize-1.2.1/README.md` & `avrotize-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,16 @@
 avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
 ```
 
 Parameters:
 - `--avsc`: The path to the Avro schema file to be converted.
 - `--python`: The path to the Python directory to write the conversion result to.
 - `--package`: (optional) The Python package name to use in the generated Python classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Python classes.
+- `--dataclasses-json-annotation`: (optional) If set, the tool will add dataclasses-json annotations to the Python classes
 
 Conversion notes:
 - The tool generates Python dataclasses (Python 3.7 or later)
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `__init__.py` file into any created
   package directories if none exists.
```

### Comparing `avrotize-1.2.1/avrotize/__init__.py` & `avrotize-1.2.2/avrotize/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from .prototoavro import  convert_proto_to_avro
 from .avrotojsons import convert_avro_to_json_schema
 from .avrotokusto import convert_avro_to_kusto
 from .avrotoparquet import convert_avro_to_parquet
 from .avrotoproto import convert_avro_to_proto
 from .avrototsql import convert_avro_to_tsql
 from .avrotoxsd import convert_avro_to_xsd
-from .avrotojava import convert_avro_to_java
-from .avrotocsharp import convert_avro_to_csharp
-from .avrotopython import convert_avro_to_python
-from .avrotots import convert_avro_to_typescript
-from .avrotojs import convert_avro_to_javascript
+from .avrotojava import convert_avro_to_java, convert_avro_schema_to_java
+from .avrotocsharp import convert_avro_to_csharp, convert_avro_schema_to_csharp
+from .avrotopython import convert_avro_to_python, convert_avro_schema_to_python
+from .avrotots import convert_avro_to_typescript, convert_avro_schema_to_typescript
+from .avrotojs import convert_avro_to_javascript, convert_avro_schema_to_javascript
 
 __all__ = [
     "convert_proto_to_avro",
     "convert_jsons_to_avro",
     "convert_kafka_struct_to_avro_schema",
     "convert_asn1_to_avro",
     "convert_xsd_to_avro",
@@ -27,12 +27,17 @@
     "convert_avro_to_json_schema",
     "convert_avro_to_kusto",
     "convert_avro_to_parquet",
     "convert_avro_to_proto",
     "convert_avro_to_tsql",
     "convert_avro_to_xsd",
     "convert_avro_to_java",
+    "convert_avro_schema_to_java",
     "convert_avro_to_csharp",
+    "convert_avro_schema_to_csharp",
     "convert_avro_to_python",
+    "convert_avro_schema_to_python",
     "convert_avro_to_typescript",
-    "convert_avro_to_javascript"
+    "convert_avro_schema_to_typescript",
+    "convert_avro_to_javascript",
+    "convert_avro_schema_to_javascript"
 ]
```

### Comparing `avrotize-1.2.1/avrotize/asn1toavro.py` & `avrotize-1.2.2/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotize.py` & `avrotize-1.2.2/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotojava.py` & `avrotize-1.2.2/avrotize/avrotojs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,266 +1,246 @@
-""" Generates Java classes from Avro schema """
+""" Convert Avro schema to TypeScript classes """
+
 import json
 import os
-from typing import Dict, List, Union
+from typing import Any, Dict, List, Set, Union
 
 from avrotize.common import pascal
 
-INDENT = '    '
-POM_CONTENT = """<?xml version="1.0" encoding="UTF-8"?>
-<project xmlns="http://maven.apache.org/POM/4.0.0"
-    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
-    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
-    <modelVersion>4.0.0</modelVersion>
-    <groupId>com.example</groupId>
-    <artifactId>demo</artifactId>
-    <version>1.0-SNAPSHOT</version>
-    <properties>
-        <maven.compiler.source>21</maven.compiler.source>
-        <maven.compiler.target>21</maven.compiler.target>
-    </properties>
-    <dependencies>
-        <dependency>
-            <groupId>org.apache.avro</groupId>
-            <artifactId>avro</artifactId>
-            <version>1.11.3</version>
-        </dependency>
-        <dependency>
-            <groupId>com.fasterxml.jackson</groupId>
-            <artifactId>jackson-bom</artifactId>
-            <version>2.17.0</version>
-            <type>pom</type>
-        </dependency>
-    </dependencies>
-</project>
-"""
-
-
-def flatten_type_name(name: str) -> str:
-    """Strips the namespace from a name"""
-    base_name = pascal(name.replace(' ', '')).split('.')[-1].replace('>', '').replace('<', '').replace(',', '')
-    return base_name
+INDENT = ' ' * 4
 
-def is_java_reserved_word(word: str) -> bool:
-    """Checks if a word is a Java reserved word"""
+def is_javascript_reserved_word(word: str) -> bool:
+    """ Check if word is a TypeScript reserved word """
     reserved_words = [
-        'abstract', 'assert', 'boolean', 'break', 'byte', 'case', 'catch', 'char', 'class', 'const',
-        'continue', 'default', 'do', 'double', 'else', 'enum', 'extends', 'final', 'finally', 'float',
-        'for', 'goto', 'if', 'implements', 'import', 'instanceof', 'int', 'interface', 'long', 'native',
-        'new', 'package', 'private', 'protected', 'public', 'return', 'short', 'static', 'strictfp',
-        'super', 'switch', 'synchronized', 'this', 'throw', 'throws', 'transient', 'try', 'void', 'volatile',
-        'while', 'true', 'false', 'null'
+        'break', 'case', 'catch', 'class', 'const', 'continue', 'debugger',
+        'default', 'delete', 'do', 'else', 'export', 'extends', 'finally',
+        'for', 'function', 'if', 'import', 'in', 'instanceof', 'new', 'return',
+        'super', 'switch', 'this', 'throw', 'try', 'typeof', 'var', 'void',
+        'while', 'with', 'yield'
     ]
     return word in reserved_words
 
-class AvroToJava:
-    """Converts Avro schema to Java classes, including Jackson annotations and Avro SpecificRecord methods"""
-    def __init__(self, base_package: str = '') -> None:
-        self.base_package = base_package.replace('.', '/')
+def is_javascript_primitive(word: str) -> bool:
+    """ Check if word is a TypeScript primitive """
+    primitives = ['null', 'boolean', 'number', 'string', 'Date']
+    return word in primitives
+
+class AvroToJavaScript:
+    """ Convert Avro schema to TypeScript classes """
+    
+    def __init__(self, base_package: str = '', avro_annotation=False) -> None:
+        self.base_package = base_package
+        self.avro_annotation = avro_annotation
         self.output_dir = os.getcwd()
-        self.avro_annotation = False
-        self.jackson_annotations = False
-        self.pascal_properties = False
-
-    def concat_package(self, package: str, name: str) -> str:
-        """Concatenates package and name using a dot separator"""
-        return f"{package}.{name}" if package else name
-
-    class JavaType:
-        """Java type definition"""
-        def __init__(self, type_name: str, union_types: List['AvroToJava.JavaType'] | None = None):
-            self.type_name = type_name
-            self.union_types = union_types
-            
-    def map_primitive_to_java(self, avro_type: str) -> JavaType:
-        """Maps Avro primitive types to Java types"""
+
+    def map_primitive_to_javascript(self, avro_type: str) -> str:
+        """ Map Avro primitive type to TypeScript type """
         mapping = {
-            'null': 'Void',
-            'boolean': 'Boolean',
-            'int': 'Integer',
-            'long': 'Long',
-            'float': 'Float',
-            'double': 'Double',
-            'bytes': 'byte[]',
-            'string': 'String',
+            'null': 'null',
+            'boolean': 'boolean',
+            'int': 'number',
+            'long': 'number',
+            'float': 'number',
+            'double': 'number',
+            'bytes': 'string',
+            'string': 'string',
         }
-        return AvroToJava.JavaType(mapping.get(avro_type, 'Object'))
+        return mapping.get(avro_type, avro_type)
+
+    def convert_logical_type_to_javascript(self, avro_type: Dict) -> str:
+        """ Convert Avro logical type to TypeScript type """
+        if 'logicalType' in avro_type:
+            if avro_type['logicalType'] in ['decimal', 'uuid']:
+                return 'string'
+            if avro_type['logicalType'] in ['date', 'time-millis', 'time-micros', 'timestamp-millis', 'timestamp-micros']:
+                return 'Date'
+            if avro_type['logicalType'] == 'duration':
+                return 'string'
+        return 'any'
     
+    def is_javascript_primitive(self, avro_type: str) -> bool:
+        """ Check if Avro type is a TypeScript primitive """
+        return avro_type in ['null', 'boolean', 'number', 'string', 'Date']
 
-    def convert_avro_type_to_java(self, avro_type: Union[str, Dict, List], parent_package: str) -> JavaType:
-        """Converts Avro type to Java type"""
+    def convert_avro_type_to_javascript(self, avro_type: Union[str, Dict, List], parent_namespace: str, import_types: set) -> str | List[Any]:
+        """ Convert Avro type to TypeScript type """
         if isinstance(avro_type, str):
-            return self.map_primitive_to_java(avro_type)
+            mapped_type = self.map_primitive_to_javascript(avro_type)
+            if mapped_type == avro_type and not self.is_javascript_primitive(mapped_type):
+                import_types.add(mapped_type)
+                return pascal(mapped_type.split('.')[-1])
+            return mapped_type
         elif isinstance(avro_type, list):
-            non_null_types = [t for t in avro_type if t != 'null']
-            if len(non_null_types) == 1:
-                return self.convert_avro_type_to_java(non_null_types[0], parent_package)
-            else:
-                types : List[AvroToJava.JavaType]  = [self.convert_avro_type_to_java(t, parent_package) for t in non_null_types]
-                return AvroToJava.JavaType('Object', types)
+            return [self.convert_avro_type_to_javascript(t, parent_namespace, import_types) for t in avro_type]
         elif isinstance(avro_type, dict):
-            if avro_type['type'] in ['record', 'enum']:
-                return self.generate_class_or_enum(avro_type, parent_package, write_file=True)
-            elif avro_type['type'] == 'array':
-                return AvroToJava.JavaType(f"List<{self.convert_avro_type_to_java(avro_type['items'], parent_package).type_name}>")
-            elif avro_type['type'] == 'map':
-                return AvroToJava.JavaType(f"Map<String, {self.convert_avro_type_to_java(avro_type['values'], parent_package).type_name}>")
-            return self.convert_avro_type_to_java(avro_type['type'], parent_package)
-        return 'Object'
-
-    def generate_class_or_enum(self, avro_schema: Dict, parent_package: str, write_file: bool = True) -> JavaType:
-        """ Generates a Java class or enum from an Avro schema """
-        if avro_schema['type'] == 'record':
-            return self.generate_class(avro_schema, parent_package, write_file)
-        elif avro_schema['type'] == 'enum':
-            return self.generate_enum(avro_schema, parent_package, write_file)
-        return AvroToJava.JavaType('Object')
-
-    def generate_class(self, avro_schema: Dict, parent_package: str, write_file: bool) -> JavaType:
-        """ Generates a Java class from an Avro record schema """
-        class_definition = ''
-        if 'doc' in avro_schema:
-            class_definition += f"/** {avro_schema['doc']} */\n"
-        package = self.concat_package(self.base_package, avro_schema.get('namespace', '').replace('.', '/')).lower()
+            if 'type' in avro_type and avro_type['type'] == 'record':
+                class_ref = self.generate_class(avro_type, parent_namespace)
+                import_types.add(class_ref)
+                return class_ref.split('.')[-1]
+            elif 'type' in avro_type and avro_type['type'] == 'enum':
+                enum_ref = self.generate_enum(avro_type, parent_namespace)
+                import_types.add(enum_ref)
+                return enum_ref.split('.')[-1]
+            elif 'type' in avro_type and avro_type['type'] == 'array':
+                return [self.convert_avro_type_to_javascript(avro_type["items"], parent_namespace, import_types)]
+            if 'type' in avro_type and avro_type['type'] == 'map':
+                return [self.convert_avro_type_to_javascript(avro_type["values"], parent_namespace, import_types)]
+            if 'logicalType' in avro_type:
+                return self.convert_logical_type_to_javascript(avro_type)
+            return self.convert_avro_type_to_javascript(avro_type['type'], parent_namespace, import_types)
+        return 'any'
+
+    def generate_class(self, avro_schema: Dict, parent_namespace: str) -> str:
+        """ Generate TypeScript class from Avro record """
+        
+        def add_check(arr_check, ft):
+            if isinstance(ft, list):
+                for ft2 in ft:
+                    add_check(arr_check, ft2)                
+            elif ft == 'null':
+                arr_check.append('v !== null')
+            elif is_javascript_primitive(ft):
+                arr_check.append(f'typeof v !== "{ft}"')
+            else:
+                arr_check.append(f'!(v instanceof {ft})')
+        
+        import_types: Set[str] = set()
         class_name = pascal(avro_schema['name'])
-        fields_str = [self.generate_property(field, parent_package) for field in avro_schema.get('fields', [])]
-        class_body = "\n".join(fields_str)
-        class_definition += f"public class {class_name}"
-        if self.avro_annotation:
-            class_definition += " implements SpecificRecord"
-        class_definition += " {\n"
-        class_definition += class_body
+        namespace = avro_schema.get('namespace', '')
+        if not namespace and parent_namespace:
+            namespace = parent_namespace
+        if self.base_package:
+            namespace = f'{self.base_package}.{namespace}'
+        fields = avro_schema.get('fields', [])
+        doc = avro_schema.get('doc', '')
+        
+        constructor_body = ''
+        class_body = ''
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             avro_schema_json = avro_schema_json.replace('"', '§')           
-            avro_schema_json = f"\"+\n{INDENT}\"".join([avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
+            avro_schema_json = f"\"+\n{' '*8}\"".join([avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
-            class_definition += f"\n\n{INDENT}public static Schema AvroSchema = new Schema.Parser().parse(\n{INDENT}\"{avro_schema_json}\");\n"
-            class_definition += f"\n{INDENT}@Override\n{INDENT}public Schema getSchema(){{ return AvroSchema; }}\n"            
-            class_definition += self.generate_get_method(avro_schema.get('fields', []), parent_package)
-            class_definition += self.generate_put_method(avro_schema.get('fields', []), parent_package)
-        class_definition += "\n}"
-
-        if write_file:
-            self.write_to_file(package, class_name, class_definition)
-        return AvroToJava.JavaType(self.concat_package(package.replace('/', '.'), class_name))
-
-    def generate_get_method(self, fields: List[Dict], parent_package: str) -> str:
-        """ Generates the get method for SpecificRecord """
-        get_method = f"\n{INDENT}@Override\n{INDENT}public Object get(int field$) {{\n"
-        get_method += f"{INDENT * 2}switch (field$) {{\n"
-        for index, field in enumerate(fields):
-            field_name = pascal(field['name']) if self.pascal_properties else field['name']
-            get_method += f"{INDENT * 3}case {index}: return this.{field_name};\n"
-        get_method += f"{INDENT * 3}default: throw new AvroRuntimeException(\"Bad index: \" + field$);\n"
-        get_method += f"{INDENT * 2}}}\n{INDENT}}}\n"
-        return get_method
-
-    def generate_put_method(self, fields: List[Dict], parent_package: str) -> str:
-        """ Generates the put method for SpecificRecord """
-        put_method = f"\n{INDENT}@Override\n{INDENT}public void put(int field$, Object value$) {{\n"
-        put_method += f"{INDENT * 2}switch (field$) {{\n"
-        for index, field in enumerate(fields):
-            field_name = pascal(field['name']) if self.pascal_properties else field['name']
-            java_type = self.convert_avro_type_to_java(field['type'], parent_package)
-            put_method += f"{INDENT * 3}case {index}: this.{field_name} = ({java_type.type_name})value$; break;\n"
-        put_method += f"{INDENT * 3}default: throw new AvroRuntimeException(\"Bad index: \" + field$);\n"
-        put_method += f"{INDENT * 2}}}\n{INDENT}}}\n"
-        return put_method
+            class_body += f'{class_name}.AvroType = avro.parse("{avro_schema_json}");\n'
+        for field in fields:
+            field_name = field['name']
+            field_doc = field.get('doc', '')
+            field_avro_type = field['type']
+            if is_javascript_reserved_word(field_name):
+                field_name += '_'
+            field_type = self.convert_avro_type_to_javascript(field['type'], namespace, import_types)
+            if field_doc:
+                constructor_body += f'{INDENT}/** {field_doc} */\n'
+            constructor_body += f'{INDENT}_{field_name} = null;\n'
+            class_body += f'Object.defineProperty({class_name}.prototype, "{field_name}", {{\n'
+            class_body += f'{INDENT}get: function() {{'+'\n'
+            class_body += f'{INDENT}{INDENT}return this._{field_name};\n'
+            class_body += f'{INDENT}}},\n'
+            class_body += f'{INDENT}set: function(value) {{'+'\n'
+            type_check = []
+            if field_avro_type == 'array':
+                arr = '!Array.isArray(value) || value.some(v => '
+                arr_check: List[str] = []
+                for ft in field_type if isinstance(field_type, list) else [field_type]:
+                    add_check(arr_check, ft)
+                arr += ' || '.join(arr_check) + ')'
+                type_check.append(arr)
+            elif field_avro_type == 'map':
+                map = '!Object.entries(value).every(([k, v]) => typeof k === "string" && '
+                map_check: List[str] = []
+                for ft in field_type if isinstance(field_type, list) else [field_type]:
+                    add_check(map_check, ft)
+                map += ' && '.join(map_check) + ')'
+                type_check.append(map)
+            else:
+                for ft in field_type if isinstance(field_type, list) else [field_type]:
+                    add_check(type_check, ft)
+            class_body += f'{INDENT}{INDENT}if ( {" && ".join(type_check)} ) throw new Error(`Invalid type for {field_name}. Expected {field_type}, got ${{value}}`);\n'
+            class_body += f'{INDENT}{INDENT}this._{field_name} = value;\n'
+            class_body += f'{INDENT}}}'+'\n'
+            class_body += '});\n\n'
+        
+        imports = ''
+        if self.avro_annotation:
+            imports += "var avro = require('avro-js');\n"
+        for import_type in import_types:
+            import_type_package = import_type.rsplit('.',1)[0]
+            import_type_type = pascal(import_type.split('.')[-1])
+            import_type_package = import_type_package.replace('.', '/')
+            namespace_path = namespace.replace('.', '/')
+            
+            if import_type_package:# get the relative path from the namespace to the import_type_package
+                import_type_package = os.path.relpath(import_type_package, namespace_path).replace(os.sep, '/')
+                if not import_type_package.startswith('.'):
+                    import_type_package = f'./{import_type_package}'
+                imports += f"var {import_type_type} = require('{import_type_package}/{import_type_type}').{import_type_type};\n"
+            else:
+                imports += f"var {import_type_type} = require('{import_type_type}'){import_type_type};\n"
+        
+        class_definition = imports + '\n'
+        if doc:
+            class_definition += f'/** {doc} */\n'        
+        class_definition += f"function {class_name}() {{\n{constructor_body}}}\n\n{class_body}\nmodule.exports = {class_name};\n"
+        self.write_to_file(namespace, class_name, class_definition)
+        return f'{namespace}.{class_name}'
 
-    def generate_enum(self, avro_schema: Dict, parent_package: str, write_file: bool) -> JavaType:
-        """ Generates a Java enum from an Avro enum schema """
-        enum_definition = ''
-        if 'doc' in avro_schema:
-            enum_definition += f"/** {avro_schema['doc']} */\n"
-        package = self.concat_package(self.base_package, avro_schema.get('namespace', '').replace('.', '/')).lower()
+    def generate_enum(self, avro_schema: Dict, parent_namespace: str) -> str:
+        """ Generate TypeScript enum from Avro enum """
         enum_name = pascal(avro_schema['name'])
+        namespace = avro_schema.get('namespace', '')
+        if not namespace and parent_namespace:
+            namespace = parent_namespace
+        if self.base_package:
+            namespace = f'{self.base_package}.{namespace}'
         symbols = avro_schema.get('symbols', [])
-        symbols_str = ', '.join(symbols)
-        enum_definition += f"public enum {enum_name} {{\n"
-        enum_definition += f"{INDENT}{symbols_str};\n"
-        enum_definition += "}\n"
-        if write_file:
-            self.write_to_file(package, enum_name, enum_definition)
-        return AvroToJava.JavaType(self.concat_package(package.replace('/', '.'), enum_name))       
         
-
-    def generate_property(self, field: Dict, parent_package: str) -> str:
-        """ Generates a Java property definition """
-        field_type = self.convert_avro_type_to_java(field['type'], parent_package)
-        field_name = pascal(field['name']) if self.pascal_properties else field['name']
-        if is_java_reserved_word(field_name):
-            field_name += "_"
-        property_def = ''
-        if 'doc' in field:
-            property_def += f"{INDENT}/** {field['doc']} */\n"
-        if self.jackson_annotations:
-            property_def += f"{INDENT}@JsonProperty(\"{field['name']}\")\n"
-        property_def += f"{INDENT}private {field_type.type_name} {field_name};\n"
-        property_def += f"{INDENT}public {field_type.type_name} get{field_name.capitalize()}() {{ return {field_name}; }}\n"
-        property_def += f"{INDENT}public void set{field_name.capitalize()}({field_type.type_name} {field_name}) {{ this.{field_name} = {field_name}; }}\n"
-        if field_type.union_types:
-            for union_type in field_type.union_types:
-                property_def += f"{INDENT}public {union_type.type_name} get{field_name.capitalize()}As{flatten_type_name(union_type.type_name)}() {{ return ({union_type.type_name}){field_name}; }}\n"
-                property_def += f"{INDENT}public void set{field_name.capitalize()}As{flatten_type_name(union_type.type_name)}({union_type.type_name} {field_name}) {{ this.{field_name} = {field_name}; }}\n"
-        return property_def
-
-    def write_to_file(self, package: str, name: str, definition: str):
-        """ Writes a Java class or enum to a file """
-        directory_path = os.path.join(self.output_dir, package)
+        enum_body = ''
+        for symbol in symbols:
+            if is_javascript_reserved_word(symbol):
+                symbol += '_'
+            enum_body += f'{INDENT}{symbol}: "{symbol}",\n'
+            
+        enum_definition = ''
+        if 'doc' in avro_schema:
+            enum_definition += f"/** {avro_schema['doc']} */\n"
+        enum_definition += f"const {enum_name} = Object.freeze({{\n{enum_body}}});\n\n"
+        enum_definition += f"module.exports = {enum_name};\n"
+        self.write_to_file(namespace, enum_name, enum_definition)
+        return f'{namespace}.{enum_name}'
+
+    def write_to_file(self, namespace: str, name: str, content: str):
+        """ Write TypeScript class to file """
+        directory_path = os.path.join(self.output_dir, namespace.replace('.', os.sep))
         if not os.path.exists(directory_path):
             os.makedirs(directory_path)
-        file_path = os.path.join(directory_path, f"{name}.java")
-
+        
+        file_path = os.path.join(directory_path, f"{name}.js")
         with open(file_path, 'w', encoding='utf-8') as file:
-            if package:
-                file.write(f"package {package.replace('/', '.')};\n\n")
-                file.write("import java.util.List;\n")
-                file.write("import java.util.Map;\n")
-            if self.avro_annotation:
-                file.write("import org.apache.avro.specific.SpecificRecord;\n")
-                file.write("import org.apache.avro.AvroRuntimeException;\n")
-                file.write("import org.apache.avro.Schema;\n")
-            if self.jackson_annotations:
-                file.write("import com.fasterxml.jackson.annotation.JsonProperty;\n")
-            file.write("\n")
-            file.write(definition)
-
-    def convert(self, avro_schema_path: str, output_dir: str):
-        """Converts Avro schema to Java"""
-        with open(avro_schema_path, 'r', encoding='utf-8') as file:
-            schema = json.load(file)
+            file.write(content)
 
+    def convert_schema(self, schema: List|Dict, output_dir: str):
+        """ Convert Avro schema to TypeScript classes """
+        self.output_dir = output_dir
         if isinstance(schema, dict):
             schema = [schema]
 
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
-        pom_path = os.path.join(output_dir, "pom.xml")
-        if not os.path.exists(pom_path):
-            with open(pom_path, 'w', encoding='utf-8') as file:
-                file.write(POM_CONTENT)
-        
-        output_dir = os.path.join(output_dir, "src/main/java".replace('/', os.sep))
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
-        self.output_dir = output_dir
         for avro_schema in schema:
-            self.generate_class_or_enum(avro_schema, self.base_package)
-                    
-
+            if avro_schema['type'] == 'record':
+                self.generate_class(avro_schema, self.base_package)
+            elif avro_schema['type'] == 'enum':
+                self.generate_enum(avro_schema, self.base_package)
+                
+    def convert(self, avro_schema_path: str, output_dir: str):
+        """ Convert Avro schema to TypeScript classes """
+        with open(avro_schema_path, 'r', encoding='utf-8') as file:
+            schema = json.load(file)
+        self.convert_schema(schema, output_dir)
 
-def convert_avro_to_java(avro_schema_path, java_file_path, package_name = '', pascal_properties=False, jackson_annotation=False, avro_annotation=False):
-    """_summary_
+def convert_avro_to_javascript(avro_schema_path, js_dir_path, package_name='', avro_annotation=False):
+    """ Convert Avro schema to TypeScript classes """
+    converter = AvroToJavaScript(package_name, avro_annotation=avro_annotation)
+    converter.convert(avro_schema_path, js_dir_path)
     
-    Converts Avro schema to C# classes
-
-    Args:
-        avro_schema_path (_type_): Avro input schema path  
-        cs_file_path (_type_): Output C# file path 
-    """
-    avrotojava = AvroToJava()
-    avrotojava.base_package = package_name
-    avrotojava.pascal_properties = pascal_properties
-    avrotojava.avro_annotation = avro_annotation
-    avrotojava.jackson_annotations = jackson_annotation
-    avrotojava.convert(avro_schema_path, java_file_path)
+def convert_avro_schema_to_javascript(avro_schema, js_dir_path, package_name='', avro_annotation=False):
+    """ Convert Avro schema to TypeScript classes """
+    converter = AvroToJavaScript(package_name, avro_annotation=avro_annotation)
+    converter.convert_schema(avro_schema, js_dir_path)
```

### Comparing `avrotize-1.2.1/avrotize/avrotojs.py` & `avrotize-1.2.2/avrotize/avrotots.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,189 +1,151 @@
 """ Convert Avro schema to TypeScript classes """
 
 import json
 import os
-from typing import Any, Dict, List, Set, Union
+from typing import Dict, List, Set, Union
 
 from avrotize.common import pascal
 
-INDENT = ' ' * 4
-
-def is_javascript_reserved_word(word: str) -> bool:
+def is_typescript_reserved_word(word: str) -> bool:
     """ Check if word is a TypeScript reserved word """
     reserved_words = [
         'break', 'case', 'catch', 'class', 'const', 'continue', 'debugger',
         'default', 'delete', 'do', 'else', 'export', 'extends', 'finally',
         'for', 'function', 'if', 'import', 'in', 'instanceof', 'new', 'return',
         'super', 'switch', 'this', 'throw', 'try', 'typeof', 'var', 'void',
         'while', 'with', 'yield'
     ]
     return word in reserved_words
 
-def is_javascript_primitive(word: str) -> bool:
-    """ Check if word is a TypeScript primitive """
-    primitives = ['null', 'boolean', 'number', 'string', 'Date']
-    return word in primitives
-
-class AvroToJavaScript:
+class AvroToTypeScript:
     """ Convert Avro schema to TypeScript classes """
     
-    def __init__(self, base_package: str = '', avro_annotation=False) -> None:
+    def __init__(self, base_package: str = '', typed_json_annotation=False, avro_annotation=False) -> None:
         self.base_package = base_package
+        self.typed_json_annotation = typed_json_annotation
         self.avro_annotation = avro_annotation
         self.output_dir = os.getcwd()
 
-    def map_primitive_to_javascript(self, avro_type: str) -> str:
+    def map_primitive_to_typescript(self, avro_type: str) -> str:
         """ Map Avro primitive type to TypeScript type """
         mapping = {
             'null': 'null',
             'boolean': 'boolean',
             'int': 'number',
             'long': 'number',
             'float': 'number',
             'double': 'number',
             'bytes': 'string',
             'string': 'string',
         }
         return mapping.get(avro_type, avro_type)
 
-    def convert_logical_type_to_javascript(self, avro_type: Dict) -> str:
+    def convert_logical_type_to_typescript(self, avro_type: Dict) -> str:
         """ Convert Avro logical type to TypeScript type """
         if 'logicalType' in avro_type:
             if avro_type['logicalType'] in ['decimal', 'uuid']:
                 return 'string'
             if avro_type['logicalType'] in ['date', 'time-millis', 'time-micros', 'timestamp-millis', 'timestamp-micros']:
                 return 'Date'
             if avro_type['logicalType'] == 'duration':
                 return 'string'
         return 'any'
     
-    def is_javascript_primitive(self, avro_type: str) -> bool:
+    def is_typescript_primitive(self, avro_type: str) -> bool:
         """ Check if Avro type is a TypeScript primitive """
         return avro_type in ['null', 'boolean', 'number', 'string', 'Date']
 
-    def convert_avro_type_to_javascript(self, avro_type: Union[str, Dict, List], parent_namespace: str, import_types: set) -> str | List[Any]:
+    def convert_avro_type_to_typescript(self, avro_type: Union[str, Dict, List], parent_namespace: str, import_types: set) -> str:
         """ Convert Avro type to TypeScript type """
         if isinstance(avro_type, str):
-            mapped_type = self.map_primitive_to_javascript(avro_type)
-            if mapped_type == avro_type and not self.is_javascript_primitive(mapped_type):
+            mapped_type = self.map_primitive_to_typescript(avro_type)
+            if mapped_type == avro_type and not self.is_typescript_primitive(mapped_type):
                 import_types.add(mapped_type)
                 return pascal(mapped_type.split('.')[-1])
             return mapped_type
         elif isinstance(avro_type, list):
-            return [self.convert_avro_type_to_javascript(t, parent_namespace, import_types) for t in avro_type]
+            types = [self.convert_avro_type_to_typescript(t, parent_namespace, import_types) for t in avro_type if t != 'null']
+            if len(types) == 1 and 'null' in avro_type:
+                return f'{types[0]} | null'
+            return ' | '.join(types)
         elif isinstance(avro_type, dict):
             if 'type' in avro_type and avro_type['type'] == 'record':
                 class_ref = self.generate_class(avro_type, parent_namespace)
                 import_types.add(class_ref)
                 return class_ref.split('.')[-1]
             elif 'type' in avro_type and avro_type['type'] == 'enum':
                 enum_ref = self.generate_enum(avro_type, parent_namespace)
                 import_types.add(enum_ref)
                 return enum_ref.split('.')[-1]
             elif 'type' in avro_type and avro_type['type'] == 'array':
-                return [self.convert_avro_type_to_javascript(avro_type["items"], parent_namespace, import_types)]
+                return f'{self.convert_avro_type_to_typescript(avro_type["items"], parent_namespace, import_types)}[]'
             if 'type' in avro_type and avro_type['type'] == 'map':
-                return [self.convert_avro_type_to_javascript(avro_type["values"], parent_namespace, import_types)]
+                return f'{{ [key: string]: {self.convert_avro_type_to_typescript(avro_type["values"], parent_namespace, import_types)} }}'
             if 'logicalType' in avro_type:
-                return self.convert_logical_type_to_javascript(avro_type)
-            return self.convert_avro_type_to_javascript(avro_type['type'], parent_namespace, import_types)
+                return self.convert_logical_type_to_typescript(avro_type)
+            return self.convert_avro_type_to_typescript(avro_type['type'], parent_namespace, import_types)
         return 'any'
 
     def generate_class(self, avro_schema: Dict, parent_namespace: str) -> str:
         """ Generate TypeScript class from Avro record """
-        
-        def add_check(arr_check, ft):
-            if isinstance(ft, list):
-                for ft2 in ft:
-                    add_check(arr_check, ft2)                
-            elif ft == 'null':
-                arr_check.append('v !== null')
-            elif is_javascript_primitive(ft):
-                arr_check.append(f'typeof v !== "{ft}"')
-            else:
-                arr_check.append(f'!(v instanceof {ft})')
-        
         import_types: Set[str] = set()
         class_name = pascal(avro_schema['name'])
         namespace = avro_schema.get('namespace', '')
         if not namespace and parent_namespace:
             namespace = parent_namespace
         if self.base_package:
             namespace = f'{self.base_package}.{namespace}'
         fields = avro_schema.get('fields', [])
         doc = avro_schema.get('doc', '')
         
-        constructor_body = ''
         class_body = ''
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             avro_schema_json = avro_schema_json.replace('"', '§')           
             avro_schema_json = f"\"+\n{' '*8}\"".join([avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
-            class_body += f'{class_name}.AvroType = avro.parse("{avro_schema_json}");\n'
+            class_body += f'    static AvroType : Type = avro.parse("{avro_schema_json}");\n'
         for field in fields:
             field_name = field['name']
             field_doc = field.get('doc', '')
-            field_avro_type = field['type']
-            if is_javascript_reserved_word(field_name):
+            if is_typescript_reserved_word(field_name):
                 field_name += '_'
-            field_type = self.convert_avro_type_to_javascript(field['type'], namespace, import_types)
+            field_type = self.convert_avro_type_to_typescript(field['type'], namespace, import_types)
             if field_doc:
-                constructor_body += f'{INDENT}/** {field_doc} */\n'
-            constructor_body += f'{INDENT}_{field_name} = null;\n'
-            class_body += f'Object.defineProperty({class_name}.prototype, "{field_name}", {{\n'
-            class_body += f'{INDENT}get: function() {{'+'\n'
-            class_body += f'{INDENT}{INDENT}return this._{field_name};\n'
-            class_body += f'{INDENT}}},\n'
-            class_body += f'{INDENT}set: function(value) {{'+'\n'
-            type_check = []
-            if field_avro_type == 'array':
-                arr = '!Array.isArray(value) || value.some(v => '
-                arr_check: List[str] = []
-                for ft in field_type if isinstance(field_type, list) else [field_type]:
-                    add_check(arr_check, ft)
-                arr += ' || '.join(arr_check) + ')'
-                type_check.append(arr)
-            elif field_avro_type == 'map':
-                map = '!Object.entries(value).every(([k, v]) => typeof k === "string" && '
-                map_check: List[str] = []
-                for ft in field_type if isinstance(field_type, list) else [field_type]:
-                    add_check(map_check, ft)
-                map += ' && '.join(map_check) + ')'
-                type_check.append(map)
-            else:
-                for ft in field_type if isinstance(field_type, list) else [field_type]:
-                    add_check(type_check, ft)
-            class_body += f'{INDENT}{INDENT}if ( {" && ".join(type_check)} ) throw new Error(`Invalid type for {field_name}. Expected {field_type}, got ${{value}}`);\n'
-            class_body += f'{INDENT}{INDENT}this._{field_name} = value;\n'
-            class_body += f'{INDENT}}}'+'\n'
-            class_body += '});\n\n'
+                class_body += f'    /** {field_doc} */\n'
+            if self.typed_json_annotation:
+                class_body += '    @jsonMember\n'
+            class_body += f'    {field_name}: {field_type};\n'
         
         imports = ''
+        if self.typed_json_annotation:
+            imports += "import { jsonObject, jsonMember } from 'typedjson';\n"
         if self.avro_annotation:
-            imports += "var avro = require('avro-js');\n"
+            imports += "import { avro, Type } from 'avro-js';\n"
         for import_type in import_types:
             import_type_package = import_type.rsplit('.',1)[0]
             import_type_type = pascal(import_type.split('.')[-1])
             import_type_package = import_type_package.replace('.', '/')
             namespace_path = namespace.replace('.', '/')
             
             if import_type_package:# get the relative path from the namespace to the import_type_package
                 import_type_package = os.path.relpath(import_type_package, namespace_path).replace(os.sep, '/')
                 if not import_type_package.startswith('.'):
                     import_type_package = f'./{import_type_package}'
-                imports += f"var {import_type_type} = require('{import_type_package}/{import_type_type}').{import_type_type};\n"
+                imports += f"import {{ {import_type_type} }} from '{import_type_package}/{import_type_type}';\n"
             else:
-                imports += f"var {import_type_type} = require('{import_type_type}'){import_type_type};\n"
+                imports += f"import {{ {import_type_type} }} from '.{import_type_type}';\n"
         
         class_definition = imports + '\n'
         if doc:
             class_definition += f'/** {doc} */\n'        
-        class_definition += f"function {class_name}() {{\n{constructor_body}}}\n\n{class_body}\nmodule.exports = {class_name};\n"
+        if self.typed_json_annotation:
+            class_definition += "@jsonObject\n"
+        class_definition += f"export class {class_name} {{\n{class_body}}}\n"
         self.write_to_file(namespace, class_name, class_definition)
         return f'{namespace}.{class_name}'
 
     def generate_enum(self, avro_schema: Dict, parent_namespace: str) -> str:
         """ Generate TypeScript enum from Avro enum """
         enum_name = pascal(avro_schema['name'])
         namespace = avro_schema.get('namespace', '')
@@ -191,48 +153,51 @@
             namespace = parent_namespace
         if self.base_package:
             namespace = f'{self.base_package}.{namespace}'
         symbols = avro_schema.get('symbols', [])
         
         enum_body = ''
         for symbol in symbols:
-            if is_javascript_reserved_word(symbol):
+            if is_typescript_reserved_word(symbol):
                 symbol += '_'
-            enum_body += f'{INDENT}{symbol}: "{symbol}",\n'
-            
-        enum_definition = ''
-        if 'doc' in avro_schema:
-            enum_definition += f"/** {avro_schema['doc']} */\n"
-        enum_definition += f"const {enum_name} = Object.freeze({{\n{enum_body}}});\n\n"
-        enum_definition += f"module.exports = {enum_name};\n"
+            enum_body += f'    {symbol} = "{symbol}",\n'
+        
+        enum_definition = f"export enum {enum_name} {{\n{enum_body}}}\n"
         self.write_to_file(namespace, enum_name, enum_definition)
         return f'{namespace}.{enum_name}'
 
     def write_to_file(self, namespace: str, name: str, content: str):
         """ Write TypeScript class to file """
         directory_path = os.path.join(self.output_dir, namespace.replace('.', os.sep))
         if not os.path.exists(directory_path):
             os.makedirs(directory_path)
         
-        file_path = os.path.join(directory_path, f"{name}.js")
+        file_path = os.path.join(directory_path, f"{name}.ts")
         with open(file_path, 'w', encoding='utf-8') as file:
             file.write(content)
 
-    def convert(self, avro_schema_path: str, output_dir: str):
+    def convert_schema(self, schema: List|Dict, output_dir: str):
         """ Convert Avro schema to TypeScript classes """
-        with open(avro_schema_path, 'r', encoding='utf-8') as file:
-            schema = json.load(file)
-
         self.output_dir = output_dir
         if isinstance(schema, dict):
             schema = [schema]
-
         for avro_schema in schema:
             if avro_schema['type'] == 'record':
                 self.generate_class(avro_schema, self.base_package)
             elif avro_schema['type'] == 'enum':
                 self.generate_enum(avro_schema, self.base_package)
+                
+    def convert(self, avro_schema_path: str, output_dir: str):
+        """ Convert Avro schema to TypeScript classes """
+        with open(avro_schema_path, 'r', encoding='utf-8') as file:
+            schema = json.load(file)
+        self.convert_schema(schema, output_dir)
 
-def convert_avro_to_javascript(avro_schema_path, js_dir_path, package_name='', avro_annotation=False):
+def convert_avro_to_typescript(avro_schema_path, js_dir_path, package_name='', typedjson_annotation=False, avro_annotation=False):
     """ Convert Avro schema to TypeScript classes """
-    converter = AvroToJavaScript(package_name, avro_annotation=avro_annotation)
+    converter = AvroToTypeScript(package_name, typed_json_annotation=typedjson_annotation, avro_annotation=avro_annotation)
     converter.convert(avro_schema_path, js_dir_path)
+    
+def convert_avro_schema_to_typescript(avro_schema, js_dir_path, package_name='', typedjson_annotation=False, avro_annotation=False):
+    """ Convert Avro schema to TypeScript classes """
+    converter = AvroToTypeScript(package_name, typed_json_annotation=typedjson_annotation, avro_annotation=avro_annotation)
+    converter.convert_schema(avro_schema, js_dir_path)
```

### Comparing `avrotize-1.2.1/avrotize/avrotojsons.py` & `avrotize-1.2.2/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotokusto.py` & `avrotize-1.2.2/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotoparquet.py` & `avrotize-1.2.2/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotoproto.py` & `avrotize-1.2.2/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotopython.py` & `avrotize-1.2.2/avrotize/avrotopython.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.base_package = base_package
         self.dataclasses_json_annotation = dataclasses_json_annotation
         self.avro_annotation = avro_annotation
         self.output_dir = os.getcwd()
 
     def is_python_primitive(self, type: str) -> bool:
         """ Checks if a type is a Python primitive type """
-        return type in ['None', 'bool', 'int', 'float', 'str', 'bytes']        
+        return type in ['None', 'bool', 'int', 'float', 'str', 'bytes']
         
     def map_primitive_to_python(self, avro_type: str) -> str:
         """Maps Avro primitive types to Python types"""
         mapping = {
             'null': 'None',
             'boolean': 'bool',
             'int': 'int',
@@ -117,17 +117,18 @@
             package_name = f"{parent_package}.{package_name}"        
         fields = [self.generate_field(field, parent_package, import_types) for field in avro_schema.get('fields', [])]
         class_definition = f"@dataclass\nclass {class_name}:\n"
         docstring = avro_schema.get('doc', '').strip() if 'doc' in avro_schema else f'A {class_name} record.'
         class_definition += INDENT + f'"""\n{INDENT}{docstring}\n\n{INDENT}Attributes:\n'
         class_definition += ''.join([self.generate_field_docstring(field, parent_package) for field in avro_schema.get('fields', [])])
         class_definition += INDENT + '"""\n'            
-        class_definition += ''.join(fields) if fields else INDENT + "pass\n"
+        class_definition += ''.join(fields) if fields else INDENT + "\n"
         
         imports = "from dataclasses import dataclass\n"
+        local_imports = ''
         if self.avro_annotation:
             imports += 'import avro.schema\n'            
             avro_schema_json = json.dumps(avro_schema)
             avro_schema_json = avro_schema_json.replace('"', '§')           
             avro_schema_json = f"\"+\n{' '*8}\"".join([avro_schema_json[i:i+70] for i in range(0, len(avro_schema_json), 70)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
             class_definition += f'\n{INDENT}AvroType: ClassVar[avro.schema.Schema] = avro.schema.parse(\n{INDENT*2}"{avro_schema_json}");\n'        
@@ -137,20 +138,23 @@
             class_definition = class_definition.replace('@dataclass', '@dataclass_json\n@dataclass')
         for import_type in import_types:
             import_type_package = import_type.rsplit('.',1)[0]
             import_type_type = pascal(import_type.split('.')[-1])
             if import_type_package.startswith(package_name):
                 import_type_package = import_type_package[len(package_name):]
             if import_type_package:
-                imports += f"from {import_type_package}.{import_type_type} import {import_type_type}\n"
+                imp = f"from {import_type_package.lower()} import {import_type_type}\n"
+                if import_type_package.startswith('.'):
+                    local_imports += imp
+                else:
+                    imports += imp
             else:
-                imports += f"from {import_type_type} import {import_type_type}\n"        
-        class_definition = imports + '\n' + class_definition
+                local_imports += f"from .{import_type_type.lower()} import {import_type_type}\n"
+        class_definition = imports + '\n' + local_imports + '\n' + class_definition
 
-        
         if write_file:
             self.write_to_file(package_name, class_name, class_definition)
         return f'{package_name}.{class_name}' if package_name else class_name
     
     def generate_enum(self, avro_schema: Dict, parent_package: str, write_file: bool) -> str:
         """Generates a Python enum from an Avro enum schema"""
         class_name = pascal(avro_schema['name'])
@@ -189,51 +193,63 @@
         if is_python_reserved_word(field_name):
             field_name += "_"
         field_docstring = INDENT*2 + f"{field_name} ({field_type}): {field_doc}\n"
         return field_docstring
     
     def write_to_file(self, package:str, name: str, definition: str):
         """Writes a Python class to a file"""
-        directory_path = os.path.join(self.output_dir, package.replace('.', '/').replace('/', os.sep))
+        directory_path = os.path.join(self.output_dir, package.replace('.', '/').replace('/', os.sep).lower())
         if not os.path.exists(directory_path):
             os.makedirs(directory_path)
         
         # drop an __init.py__ file in all directories along the path above output_dir
         package_name = package
         while package_name:
-            init_file_path = os.path.join(self.output_dir, package_name.replace('.', '/').replace('/', os.sep), '__init__.py')
+            init_file_path = os.path.join(directory_path, '__init__.py')
             if not os.path.exists(init_file_path):
                 with open(init_file_path, 'w', encoding='utf-8') as file:
                     file.write('')
             if '.' in package_name:
                 package_name = package_name.rsplit('.', 1)[0]
             else:
                 package_name = ''
             
-        file_path = os.path.join(directory_path, f"{name}.py")
+        file_path = os.path.join(directory_path, f"{name.lower()}.py")
 
         with open(file_path, 'w', encoding='utf-8') as file:
             file.write(f'""" {name} """\n\n')
-            file.write("# pylint: disable-msg=C0103\n\n")
+            file.write("# pylint: disable=invalid-name,line-too-long,too-many-instance-attributes\n\n")
             
             pattern = r"(?<!\w)(Dict|List|Union|Optional|Any|ClassVar)"
             references = set(re.findall(pattern, definition))
             if references:
                 file.write(f'from typing import {",".join(references)}\n')
             file.write('\n'+definition)
 
+    def convert_schemas(self, avro_schemas: List, output_dir: str):
+        """ Converts Avro schema to Python data classes"""
+        self.output_dir = output_dir
+        for avro_schema in avro_schemas:
+            if avro_schema['type'] == 'enum':
+                self.generate_enum(avro_schema, self.base_package, write_file=True)
+            elif avro_schema['type'] == 'record':
+                self.generate_class(avro_schema, self.base_package, write_file=True)
+    
     def convert(self, avro_schema_path: str, output_dir: str):
         """Converts Avro schema to Python data classes"""
         with open(avro_schema_path, 'r', encoding='utf-8') as file:
             schema = json.load(file)
-
         if isinstance(schema, dict):
             schema = [schema]
-
-        self.output_dir = output_dir
-        for avro_schema in schema:
-            self.generate_class(avro_schema, self.base_package, write_file=True)
+        return self.convert_schemas(schema, output_dir)
 
 def convert_avro_to_python(avro_schema_path, py_file_path, package_name = '', dataclasses_json_annotation = False, avro_annotation = False):
     """Converts Avro schema to Python data classes"""
     avro_to_python = AvroToPython(package_name, dataclasses_json_annotation=dataclasses_json_annotation, avro_annotation=avro_annotation)
     avro_to_python.convert(avro_schema_path, py_file_path)
+
+def convert_avro_schema_to_python(avro_schema, py_file_path, package_name = '', dataclasses_json_annotation = False, avro_annotation = False):
+    """Converts Avro schema to Python data classes"""
+    avro_to_python = AvroToPython(package_name, dataclasses_json_annotation=dataclasses_json_annotation, avro_annotation=avro_annotation)
+    if isinstance(avro_schema, dict):
+        avro_schema = [avro_schema]
+    avro_to_python.convert_schemas(avro_schema, py_file_path)
```

### Comparing `avrotize-1.2.1/avrotize/avrototsql.py` & `avrotize-1.2.2/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/avrotoxsd.py` & `avrotize-1.2.2/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/common.py` & `avrotize-1.2.2/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/dependency_resolver.py` & `avrotize-1.2.2/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/generic/generic.avsc` & `avrotize-1.2.2/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/jsonstoavro.py` & `avrotize-1.2.2/avrotize/jsonstoavro.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.imported_types: Dict[Any, Any] = {}
         self.root_namespace = 'example.com'
         self.max_recursion_depth = 40
         self.types_with_unmerged_types: List[dict] = []
         self.content_cache: Dict[str,str] = {}
         self.utility_namespace = 'utility.vasters.com'
         self.split_top_level_records = False
+        self.root_class_name = 'document'
 
     def is_empty_type(self, avro_type):
         """
         Check if the Avro type is an empty type.
 
         Parameters:
         avro_type (any): The Avro type to check.
@@ -1061,15 +1062,15 @@
             # we will merge allOf, oneOf, anyOf into a union record type
             type = self.json_type_to_avro_type(json_object, name, '', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack)
             if isinstance(type, str):
                 # we are skipping references and primitives
                 return None
             if isinstance(type, list):
                 # we should have a union type
-                avro_type = self.create_wrapper_record(name, self.utility_namespace, 'options', [], type)
+                avro_type = self.create_wrapper_record(name+"_union", self.utility_namespace, 'options', [], type)
             elif isinstance(type, dict) and 'type' in type and type['type'] != 'record':
                 # merge the type into a record type if it's not a record type
                 print(f'INFO: Standalone type {name} is being wrapped in a record')
                 avro_type = self.create_wrapper_record(avro_name(type.get('name',name)+'_wrapper'), self.utility_namespace, 'value', type.get('dependencies', []), type)
             else:
                 avro_type = type
             # add external dependencies to the record    
@@ -1395,15 +1396,15 @@
 
     def jsons_to_avro(self, json_schema: dict | list, namespace: str, base_uri: str) -> list | dict | str:
         """Convert a JSON-schema to an Avro-schema."""
         avro_schema: List[dict] = []
         record_stack: List[str] = []
 
         parsed_url = urlparse(base_uri)
-        schema_name = 'document'
+        schema_name = self.root_class_name
 
         if isinstance(json_schema, dict) and ('definitions' in json_schema or '$defs' in json_schema):
             # this is a swagger file or has a 'definitions' block
             json_schema_defs = json_schema.get('definitions', json_schema.get('$defs', []))
             for def_schema_name, schema in json_schema_defs.items():
                 if 'type' in schema or 'allOf' in schema or 'oneOf' in schema or 'anyOf' in schema or 'properties' in schema or 'enum' in schema or '$ref' in schema or 'additionalProperties' in schema or 'patternProperties' in schema:
                     # this is a schema definition
@@ -1511,16 +1512,18 @@
                         json.dump(item, avro_file, indent=4)
         else:
             with open(avro_schema_path, 'w') as avro_file:
                 json.dump(avro_schema, avro_file, indent=4)
         return avro_schema
     
 
-def convert_jsons_to_avro(json_schema_file_path: str, avro_schema_path: str, namespace: str = '', utility_namespace = '', split_top_level_records = False) -> list | dict | str:
+def convert_jsons_to_avro(json_schema_file_path: str, avro_schema_path: str, namespace: str = '', utility_namespace = '', root_class_name = '', split_top_level_records = False) -> list | dict | str:
     """Convert JSON schema file to Avro schema file."""
     try:
         converter = JsonToAvroConverter()
         converter.split_top_level_records = split_top_level_records
+        if root_class_name:
+            converter.root_class_name = root_class_name
         return converter.convert_jsons_to_avro(json_schema_file_path, avro_schema_path, namespace, utility_namespace)
     except Exception as e:
         print(f'Error converting JSON {json_schema_file_path} to Avro: {e.args[0]}')
         return []
```

### Comparing `avrotize-1.2.1/avrotize/kconnect.json` & `avrotize-1.2.2/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/kstructtoavro.py` & `avrotize-1.2.2/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/proto2parser.py` & `avrotize-1.2.2/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/proto3parser.py` & `avrotize-1.2.2/avrotize/proto3parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 googleoption: "option" "(google.api.http)"  "=" "{" [ "post:" CONSTANT [ "body:" CONSTANT ] ] "}" ";"
 service: [ comments ] "service" SERVICENAME "{" ( option | rpc | EMPTYSTATEMENT )* "}"
 rpc: [ comments ] "rpc" RPCNAME "(" [ "stream" ] MESSAGETYPE ")" "returns" "(" [ "stream" ] MESSAGETYPE ")" ( ( "{" ( googleoption | option | EMPTYSTATEMENT )* "}" ) | ";" )
 
 proto: [ comments ] syntax ( import | package | option | topleveldef | EMPTYSTATEMENT )*
 topleveldef: message | enum | service | comments
 
-TAIL: ";" /[\s|\t]/* [ COMMENT ] NEWLINE
+TAIL: ";" /[\s|\t]/* [ COMMENT ] [ NEWLINE ]
 COMMENT: "//" /[^\n]/*
 BLOCKCOMMENT: "/*" /./* "*/"
 comments: (( COMMENT | BLOCKCOMMENT ) NEWLINE )+
 COMMENTS: (( COMMENT | BLOCKCOMMENT ) NEWLINE )+
 
 %import common.HEXDIGIT
 %import common.DIGIT -> DECIMALDIGIT
```

### Comparing `avrotize-1.2.1/avrotize/prototoavro.py` & `avrotize-1.2.2/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/any.avsc` & `avrotize-1.2.2/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/api.avsc` & `avrotize-1.2.2/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/duration.avsc` & `avrotize-1.2.2/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/field_mask.avsc` & `avrotize-1.2.2/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/struct.avsc` & `avrotize-1.2.2/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/timestamp.avsc` & `avrotize-1.2.2/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/type.avsc` & `avrotize-1.2.2/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/prototypes/wrappers.avsc` & `avrotize-1.2.2/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/avrotize/xsdtoavro.py` & `avrotize-1.2.2/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/pyproject.toml` & `avrotize-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.1/PKG-INFO` & `avrotize-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -486,14 +486,16 @@
 avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
 ```
 
 Parameters:
 - `--avsc`: The path to the Avro schema file to be converted.
 - `--python`: The path to the Python directory to write the conversion result to.
 - `--package`: (optional) The Python package name to use in the generated Python classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Python classes.
+- `--dataclasses-json-annotation`: (optional) If set, the tool will add dataclasses-json annotations to the Python classes
 
 Conversion notes:
 - The tool generates Python dataclasses (Python 3.7 or later)
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `__init__.py` file into any created
   package directories if none exists.
```

