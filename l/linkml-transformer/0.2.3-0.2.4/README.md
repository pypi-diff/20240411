# Comparing `tmp/linkml_transformer-0.2.3.tar.gz` & `tmp/linkml_transformer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_transformer-0.2.3.tar", max compression
+gzip compressed data, was "linkml_transformer-0.2.4.tar", max compression
```

## Comparing `linkml_transformer-0.2.3.tar` & `linkml_transformer-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    10030 2024-01-18 02:15:49.593365 linkml_transformer-0.2.3/README.md
--rw-r--r--   0        0        0     1229 2024-01-18 02:16:18.673192 linkml_transformer-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      135 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/cli/__init__.py
--rw-r--r--   0        0        0     6220 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/cli/cli.py
--rw-r--r--   0        0        0       61 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/__init__.py
--rw-r--r--   0        0        0      463 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/awk_compiler.py
--rw-r--r--   0        0        0     2675 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/compiler.py
--rw-r--r--   0        0        0     3869 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/graphviz_compiler.py
--rw-r--r--   0        0        0     1290 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/j2_based_compiler.py
--rw-r--r--   0        0        0      276 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/markdown_compiler.py
--rw-r--r--   0        0        0     3547 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/python_compiler.py
--rw-r--r--   0        0        0      399 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/r2rml_compiler.py
--rw-r--r--   0        0        0      411 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/sparql_compiler.py
--rw-r--r--   0        0        0      427 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/sql_compiler.py
--rw-r--r--   0        0        0      476 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/sssom_compiler.py
--rw-r--r--   0        0        0       63 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/templates/__init__.py
--rw-r--r--   0        0        0      717 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/templates/markdown.j2
--rw-r--r--   0        0        0      173 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/tr/__init__.py
--rw-r--r--   0        0        0      756 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/compiler/tr/transformer_to_mapping_tables.tr.yaml
--rw-r--r--   0        0        0      111 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/datamodel/__init__.py
--rw-r--r--   0        0        0      480 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/datamodel/specification_view.py
--rw-r--r--   0        0        0    18679 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/datamodel/transformer_model.py
--rw-r--r--   0        0        0    10593 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/datamodel/transformer_model.yaml
--rw-r--r--   0        0        0        0 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/functions/__init__.py
--rw-r--r--   0        0        0     4447 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/functions/unit_conversion.py
--rw-r--r--   0        0        0        0 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/importer/__init__.py
--rw-r--r--   0        0        0      874 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/importer/importer.py
--rw-r--r--   0        0        0        0 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/inference/__init__.py
--rw-r--r--   0        0        0     1573 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/inference/inference.py
--rw-r--r--   0        0        0     7422 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/inference/inverter.py
--rw-r--r--   0        0        0    10132 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/inference/schema_mapper.py
--rw-r--r--   0        0        0     4753 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/session.py
--rw-r--r--   0        0        0        0 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/transformer/__init__.py
--rw-r--r--   0        0        0    16635 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/transformer/object_transformer.py
--rw-r--r--   0        0        0     9658 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/transformer/transformer.py
--rw-r--r--   0        0        0        0 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/utils/__init__.py
--rw-r--r--   0        0        0     1306 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/utils/dynamic_object.py
--rw-r--r--   0        0        0     6824 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/utils/eval_utils.py
--rw-r--r--   0        0        0      783 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/utils/loaders.py
--rw-r--r--   0        0        0     9510 2024-01-18 02:15:49.597365 linkml_transformer-0.2.3/src/linkml_transformer/utils/multi_file_transformer.py
--rw-r--r--   0        0        0    10679 1970-01-01 00:00:00.000000 linkml_transformer-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1676 2024-04-11 01:48:48.849817 linkml_transformer-0.2.4/README.md
+-rw-r--r--   0        0        0     1345 2024-04-11 01:49:19.417782 linkml_transformer-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/cli/__init__.py
+-rw-r--r--   0        0        0     6222 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/cli/cli.py
+-rw-r--r--   0        0        0       61 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/__init__.py
+-rw-r--r--   0        0        0      463 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/awk_compiler.py
+-rw-r--r--   0        0        0     2809 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/compiler.py
+-rw-r--r--   0        0        0     3869 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/graphviz_compiler.py
+-rw-r--r--   0        0        0     1290 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/j2_based_compiler.py
+-rw-r--r--   0        0        0      276 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/markdown_compiler.py
+-rw-r--r--   0        0        0     3547 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/python_compiler.py
+-rw-r--r--   0        0        0      399 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/r2rml_compiler.py
+-rw-r--r--   0        0        0      411 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/sparql_compiler.py
+-rw-r--r--   0        0        0     4303 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/sql_compiler.py
+-rw-r--r--   0        0        0      476 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/sssom_compiler.py
+-rw-r--r--   0        0        0       63 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/templates/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/templates/markdown.j2
+-rw-r--r--   0        0        0      173 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/tr/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/compiler/tr/transformer_to_mapping_tables.tr.yaml
+-rw-r--r--   0        0        0      111 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/datamodel/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/datamodel/sssom.map.yaml
+-rw-r--r--   0        0        0    18679 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/datamodel/transformer_model.py
+-rw-r--r--   0        0        0    10659 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/datamodel/transformer_model.yaml
+-rw-r--r--   0        0        0        0 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/functions/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/functions/unit_conversion.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/importer/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/importer/importer.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/inference/__init__.py
+-rw-r--r--   0        0        0     1573 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/inference/inference.py
+-rw-r--r--   0        0        0     7422 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/inference/inverter.py
+-rw-r--r--   0        0        0    10133 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/inference/schema_mapper.py
+-rw-r--r--   0        0        0     6658 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/session.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/transformer/__init__.py
+-rw-r--r--   0        0        0     2242 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/transformer/duckdb_transformer.py
+-rw-r--r--   0        0        0    16640 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/transformer/object_transformer.py
+-rw-r--r--   0        0        0     9844 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/transformer/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:48:48.853817 linkml_transformer-0.2.4/src/linkml_transformer/utils/__init__.py
+-rw-r--r--   0        0        0     1306 2024-04-11 01:48:48.857817 linkml_transformer-0.2.4/src/linkml_transformer/utils/dynamic_object.py
+-rw-r--r--   0        0        0     6824 2024-04-11 01:48:48.857817 linkml_transformer-0.2.4/src/linkml_transformer/utils/eval_utils.py
+-rw-r--r--   0        0        0      783 2024-04-11 01:48:48.857817 linkml_transformer-0.2.4/src/linkml_transformer/utils/loaders.py
+-rw-r--r--   0        0        0     9512 2024-04-11 01:48:48.857817 linkml_transformer-0.2.4/src/linkml_transformer/utils/multi_file_transformer.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 linkml_transformer-0.2.4/PKG-INFO
```

### Comparing `linkml_transformer-0.2.3/pyproject.toml` & `linkml_transformer-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "linkml-transformer"
-version = "v0.2.3"
+version = "v0.2.4"
 description = ""
 authors = ["cmungall <cjm@berkeleybop.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-linkml-runtime = ">=1.5.2"
+linkml-runtime = ">=1.7.2"
 asteval = "^0.9.29"
 deepdiff = "^6.7.1"
 pydantic = "^2.5.3"
 ucumvert = "^0.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-linkml = ">=1.5.0"
+linkml = ">=1.7.0"
 mkdocs-mermaid2-plugin = "^0.6.0"
+mknotebooks = "^0.8.0"
+mkdocs-windmill = "*"
+tox = "*"
 
 [tool.poetry.scripts]
 linkml-tr = "linkml_transformer.cli.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 linkml = "^1.6.7"
@@ -30,14 +33,18 @@
 [tool.poetry.group.units.dependencies]
 pint = "^0.23"
 
 
 [tool.poetry.group.graphviz.dependencies]
 graphviz = "^0.20.1"
 
+
+[tool.poetry.group.duckdb.dependencies]
+duckdb = "^0.10.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310", "py311"]
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/cli/cli.py` & `linkml_transformer-0.2.4/src/linkml_transformer/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command line interface for linkml-transformer."""
+
 import logging
 import sys
 
 import click
 
 __all__ = [
     "main",
@@ -89,15 +90,15 @@
     logging.info(f"Transforming {input} conforming to {schema} using {transformer_specification}")
     tr = ObjectTransformer(**kwargs)
     tr.source_schemaview = SchemaView(schema)
     tr.load_transformer_specification(transformer_specification)
     with open(input) as file:
         input_obj = yaml.safe_load(file)
     tr.index(input_obj, source_type)
-    tr_obj = tr.transform(input_obj, source_type)
+    tr_obj = tr.map_object(input_obj, source_type)
     if output:
         outfile = open(output, "w", encoding="utf-8")
     else:
         outfile = sys.stdout
     outfile.write(yaml_dumper.dumps(tr_obj))
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/compiler/compiler.py` & `linkml_transformer-0.2.4/src/linkml_transformer/compiler/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 - LinkML-Transformer Specifications to R2RML
 - LinkML-Transformer Specifications to awk scripts
 - LinkML-Transformer Specifications to SQL
 - LinkML-Transformer Specifications to Python (OO)
 - LinkML-Transformer Specifications to Pandas
 - LinkML-Transformer Specifications to Hamilton
 """
+
 from abc import ABC
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from types import ModuleType
 from typing import Iterator, Optional
 
 from linkml_runtime import SchemaView
 from linkml_runtime.dumpers import yaml_dumper
 from linkml_runtime.utils.compile_python import compile_python
 
 from linkml_transformer.datamodel.transformer_model import TransformationSpecification
 from linkml_transformer.inference.schema_mapper import SchemaMapper
 
 
 @dataclass
 class CompiledSpecification:
-    serialization: str
+    serialization: str = field(default="")
 
     _module: Optional[ModuleType] = None
 
     @property
     def module(self) -> ModuleType:
         if not self._module:
             self._module = compile_python(self.serialization)
@@ -43,14 +44,17 @@
     """
     Base class for all compilers.
 
     A compiler will compile a transformation specification into
     an alternative representation.
 
     An example compiler would be a R2RML compiler.
+
+    Note: Compilers and Importers will in general be implemented by providing
+    mapping specifications
     """
 
     source_schemaview: SchemaView = None
     """A view over the schema describing the source."""
 
     source_python_module: str = None
     """The python module containing the source classes."""
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/compiler/graphviz_compiler.py` & `linkml_transformer-0.2.4/src/linkml_transformer/compiler/graphviz_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/compiler/j2_based_compiler.py` & `linkml_transformer-0.2.4/src/linkml_transformer/compiler/j2_based_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/compiler/python_compiler.py` & `linkml_transformer-0.2.4/src/linkml_transformer/compiler/python_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/compiler/templates/markdown.j2` & `linkml_transformer-0.2.4/src/linkml_transformer/compiler/templates/markdown.j2`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/compiler/tr/transformer_to_mapping_tables.tr.yaml` & `linkml_transformer-0.2.4/src/linkml_transformer/compiler/tr/transformer_to_mapping_tables.tr.yaml`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/datamodel/transformer_model.py` & `linkml_transformer-0.2.4/src/linkml_transformer/datamodel/transformer_model.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/datamodel/transformer_model.yaml` & `linkml_transformer-0.2.4/src/linkml_transformer/datamodel/transformer_model.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,17 @@
         range: string
         examples:
           - value: ','
           - value: '|'
           - value: ';'
       reversed:
         range: boolean
+      over_slots:
+        range: string
+        multivalued: true
       syntax:
         range: SerializationSyntaxType
         examples:
           - value: 'json'
           - value: 'yaml'
 
   Inverse:
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/functions/unit_conversion.py` & `linkml_transformer-0.2.4/src/linkml_transformer/functions/unit_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Basic unit conversion functions.
 
 Currently only native pint units or UCUM units are supported.
 
 For UCUM, the ucumvert library is used to convert UCUM units to pint units,
 see `<https://github.com/dalito/ucumvert>`_.
 """
+
 from enum import Enum
 from functools import lru_cache
 from typing import Any, Optional
 
 import lark
 import pint
 from ucumvert import PintUcumRegistry
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/importer/importer.py` & `linkml_transformer-0.2.4/src/linkml_transformer/importer/importer.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/inference/inference.py` & `linkml_transformer-0.2.4/src/linkml_transformer/inference/inference.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/inference/inverter.py` & `linkml_transformer-0.2.4/src/linkml_transformer/inference/inverter.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/inference/schema_mapper.py` & `linkml_transformer-0.2.4/src/linkml_transformer/inference/schema_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 A SchemaMapper translates a source schema and transformation specification into a target schema.
 
 AKA profiling
 """
+
 import logging
 from collections import defaultdict
 from copy import copy
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Tuple
 
 from linkml_runtime import SchemaView
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/session.py` & `linkml_transformer-0.2.4/src/linkml_transformer/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,71 @@
 import logging
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any, Optional, Type, Union
 
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.dumpers import yaml_dumper
 from linkml_runtime.linkml_model import SchemaDefinition
+from linkml_runtime.processing.referencevalidator import ReferenceValidator
+from linkml_runtime.utils.introspection import package_schemaview
 
 from linkml_transformer import ObjectTransformer
 from linkml_transformer.datamodel.transformer_model import TransformationSpecification
 from linkml_transformer.inference.inverter import TransformationSpecificationInverter
 from linkml_transformer.inference.schema_mapper import SchemaMapper
+from linkml_transformer.transformer.transformer import Transformer
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Session:
     """
     A wrapper object for a transformer session.
+
+    TODO:
+
+    - rename to Manager?
+    - consolidate configuration
+    - include source and target database
+
+        - current spec, src_sv, tgt_sv all live in both this class and transformer
     """
 
+    transformer_specification: Optional[TransformationSpecification] = None
     source_schemaview: Optional[SchemaView] = None
+    transformer: Optional[Transformer] = None
     object_transformer: Optional[ObjectTransformer] = None
     schema_mapper: Optional[SchemaMapper] = None
     _target_schema: Optional[SchemaDefinition] = None
+    _target_schemaview: Optional[SchemaView] = None
 
-    @property
-    def transformer_specification(self) -> TransformationSpecification:
-        if self.object_transformer is None:
-            raise ValueError("No transformer specified")
-        return self.object_transformer.specification
+    def set_transformer_specification(
+        self, specification: Optional[Union[TransformationSpecification, dict, str, Path]] = None
+    ):
+        if isinstance(specification, Path):
+            specification = str(specification)
+        if isinstance(specification, TransformationSpecification):
+            self.transformer_specification = specification
+        elif isinstance(specification, dict):
+            # TODO: centralize this code
+            normalizer = ReferenceValidator(
+                package_schemaview("linkml_transformer.datamodel.transformer_model")
+            )
+            normalizer.expand_all = True
+            specification = normalizer.normalize(specification)
+            self.transformer_specification = TransformationSpecification(**specification)
+        elif isinstance(specification, str):
+            if "\n" in specification:
+                obj = yaml.safe_load(specification)
+            else:
+                obj = yaml.safe_load(open(specification))
+            self.set_transformer_specification(obj)
 
     def set_source_schema(self, schema: Union[str, Path, dict, SchemaView, SchemaDefinition]):
         """
         Sets the schema from a path or SchemaView object.
         """
         if isinstance(schema, str):
             sv = SchemaView(schema)
@@ -48,64 +78,82 @@
         elif isinstance(schema, SchemaDefinition):
             sv = SchemaView(schema)
         else:
             raise ValueError(f"Unsupported schema type: {type(schema)}")
         self.source_schemaview = sv
         self._target_schema = None
 
+    def set_transformer(
+        self,
+        transformer: Optional[Union[Transformer, Type[Transformer]]],
+        **kwargs,
+    ):
+        if isinstance(transformer, Type):
+            transformer = transformer()
+        transformer.specification = self.transformer_specification
+        self.transformer = transformer
+
     def set_object_transformer(
-        self, transformer: Optional[Union[ObjectTransformer, dict, str, Path]] = None
+        self,
+        transformer: Optional[
+            Union[ObjectTransformer, TransformationSpecification, dict, str, Path]
+        ] = None,
     ):
         if transformer is None:
             if self.object_transformer is not None:
                 logger.info("No change")
                 return
             else:
                 logger.warning("No transformer specified")
                 return
-        if isinstance(transformer, ObjectTransformer):
-            self.object_transformer = transformer
-        elif isinstance(transformer, dict):
-            self.object_transformer = ObjectTransformer()
-            self.object_transformer.create_transformer_specification(transformer)
-        elif isinstance(transformer, str):
-            self.object_transformer = ObjectTransformer()
-            self.object_transformer.create_transformer_specification(yaml.safe_load(transformer))
+        if transformer is not None:
+            if isinstance(transformer, ObjectTransformer):
+                self.object_transformer = transformer
+            else:
+                self.set_transformer_specification(transformer)
+                self.object_transformer = ObjectTransformer()
+                self.object_transformer.specification = self.transformer_specification
         self._target_schema = None
 
+    @property
     def target_schema(self) -> SchemaDefinition:
         if self._target_schema is None:
             if not self.schema_mapper:
                 self.schema_mapper = SchemaMapper(source_schemaview=self.source_schemaview)
-            self._target_schema = self.schema_mapper.derive_schema(
-                self.object_transformer.specification
-            )
+            self._target_schema = self.schema_mapper.derive_schema(self.transformer_specification)
         return self._target_schema
 
+    @property
+    def target_schemaview(self) -> SchemaView:
+        if self._target_schemaview is None:
+            # TODO: simplify
+            self._target_schemaview = SchemaView(yaml_dumper.dumps(self.target_schema))
+        return self._target_schemaview
+
     def transform(self, obj: dict, **kwargs) -> dict:
         if self.object_transformer is None:
             raise ValueError("No transformer specified")
         if not self.object_transformer.source_schemaview:
             self.object_transformer.source_schemaview = self.source_schemaview
-        return self.object_transformer.transform(obj, **kwargs)
+        return self.object_transformer.map_object(obj, **kwargs)
 
     def reverse_transform(self, obj: dict, **kwargs) -> dict:
         inv_spec = self.invert()
         reverse_transformer = ObjectTransformer()
         reverse_transformer.specification = inv_spec
-        reverse_transformer.source_schemaview = SchemaView(yaml_dumper.dumps(self.target_schema()))
-        return reverse_transformer.transform(obj, **kwargs)
+        reverse_transformer.source_schemaview = SchemaView(yaml_dumper.dumps(self.target_schema))
+        return reverse_transformer.map_object(obj, **kwargs)
 
     def invert(self, in_place=False) -> TransformationSpecification:
         """
         Invert the transformer specification.
         """
         inverter = TransformationSpecificationInverter(
             source_schemaview=self.source_schemaview,
-            target_schemaview=SchemaView(yaml_dumper.dumps(self.target_schema())),
+            target_schemaview=SchemaView(yaml_dumper.dumps(self.target_schema)),
         )
         inv_spec = inverter.invert(self.transformer_specification)
         if in_place:
             raise NotImplementedError
         return inv_spec
 
     def graphviz(self, **kwargs) -> Any:
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/transformer/object_transformer.py` & `linkml_transformer-0.2.4/src/linkml_transformer/transformer/object_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             if target is None:
                 raise ValueError(f"target must be passed if source_obj is dict: {source_obj}")
             source_obj_typed = dynamic_object(source_obj, self.source_schemaview, target)
             self.object_index = ObjectIndex(source_obj_typed, schemaview=self.source_schemaview)
         else:
             self.object_index = ObjectIndex(source_obj, schemaview=self.source_schemaview)
 
-    def transform(
+    def map_object(
         self,
         source_obj: OBJECT_TYPE,
         source_type: str = None,
         target_type: str = None,
     ) -> Union[DICT_OBJ, Any]:
         """
         Transform a source object into a target object.
@@ -170,24 +170,24 @@
                 v = source_obj.get(slot_derivation.name, None)
             if source_class_slot and v is not None:
                 # slot is mapped and there is a value in the assignment
                 target_range = slot_derivation.range
                 source_class_slot_range = source_class_slot.range
                 if source_class_slot.multivalued:
                     if isinstance(v, list):
-                        v = [self.transform(v1, source_class_slot_range, target_range) for v1 in v]
+                        v = [self.map_object(v1, source_class_slot_range, target_range) for v1 in v]
                     elif isinstance(v, dict):
                         v = {
-                            k1: self.transform(v1, source_class_slot_range, target_range)
+                            k1: self.map_object(v1, source_class_slot_range, target_range)
                             for k1, v1 in v.items()
                         }
                     else:
                         v = [v]
                 else:
-                    v = self.transform(v, source_class_slot_range, target_range)
+                    v = self.map_object(v, source_class_slot_range, target_range)
                 if (
                     self._is_coerce_to_multivalued(slot_derivation, class_deriv)
                     and v is not None
                     and not isinstance(v, list)
                 ):
                     v = self._singlevalued_to_multivalued(v, slot_derivation)
                 if self._is_coerce_to_singlevalued(slot_derivation, class_deriv) and isinstance(
@@ -338,15 +338,15 @@
         source_type_name = source_type.__name__
         # if isinstance(source_obj, YAMLRoot):
         #    source_obj_dict = json_dumper.to_dict(source_obj)
         # elif isinstance(source_obj, BaseModel):
         #    source_obj_dict = source_obj.dict()
         # else:
         #    raise ValueError(f"Do not know how to handle type: {typ}")
-        tr_obj_dict = self.transform(source_obj, source_type_name)
+        tr_obj_dict = self.map_object(source_obj, source_type_name)
         return target_class(**tr_obj_dict)
 
     def transform_enum(self, source_value: str, enum_name: str, source_obj: Any) -> Optional[str]:
         enum_deriv = self._get_enum_derivation(enum_name)
         if enum_deriv.expr:
             try:
                 if enum_deriv.expr:
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/transformer/transformer.py` & `linkml_transformer-0.2.4/src/linkml_transformer/transformer/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Transformers (aka data mappers) are used to transform objects from one class to another
 using a transformation specification.
 """
+
 import logging
 from abc import ABC
 from copy import deepcopy
 from dataclasses import dataclass, field
 from pathlib import Path
-from types import ModuleType
 from typing import Any, Dict, Optional, Union
 
 import yaml
 from curies import Converter
 from linkml_runtime import SchemaView
 from linkml_runtime.processing.referencevalidator import ReferenceValidator
 from linkml_runtime.utils.introspection import package_schemaview
@@ -42,46 +42,54 @@
     A transformer will generate an instance of a target class from
     an instance of a source class, making use of a specification.
 
     This is an abstract class. Different implementations will
     subclass this
     """
 
-    source_schemaview: SchemaView = None
-    """A view over the schema describing the input/source object."""
-
     specification: TransformationSpecification = None
     """A specification of how to generate target objects from source objects."""
 
+    source_schemaview: SchemaView = None
+    """A view over the schema describing the input/source object."""
+
     _derived_specification: TransformationSpecification = None
     """A specification with inferred missing values."""
 
     target_schemaview: Optional[SchemaView] = None
     """A view over the schema describing the output/target object."""
 
-    target_module: Optional[ModuleType] = None
-    """The python module which the target object should conform to."""
-
-    prefix_map: Optional[Dict[str, str]] = None
-    """Additional prefixes"""
-
     unrestricted_eval: bool = field(default=False)
+    """Set to True to allow arbitrary evals as part of transformation."""
 
     _curie_converter: Converter = None
 
-    def transform(self, obj: OBJECT_TYPE, source_type: str = None) -> OBJECT_TYPE:
+    def map_object(self, obj: OBJECT_TYPE, source_type: str = None, **kwargs) -> OBJECT_TYPE:
         """
         Transform source object into an instance of the target class.
 
         :param obj:
         :param source_type:
         :return:
         """
         raise NotImplementedError
 
+    def map_database(
+        self, source_database: Any, target_database: Optional[Any] = None, **kwargs
+    ) -> OBJECT_TYPE:
+        """
+        Transform source resource.
+
+        :param source_database:
+        :param target_database:
+        :param kwargs:
+        :return:
+        """
+        raise NotImplementedError
+
     def load_source_schema(self, path: Union[str, Path, dict]):
         """
         Sets source_schemaview from a schema path.
 
         :param path:
         :return:
         """
```

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/utils/dynamic_object.py` & `linkml_transformer-0.2.4/src/linkml_transformer/utils/dynamic_object.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/utils/eval_utils.py` & `linkml_transformer-0.2.4/src/linkml_transformer/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/utils/loaders.py` & `linkml_transformer-0.2.4/src/linkml_transformer/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.2.3/src/linkml_transformer/utils/multi_file_transformer.py` & `linkml_transformer-0.2.4/src/linkml_transformer/utils/multi_file_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Iterate through all examples in a folder testing them for validity.
 
 """
+
 import glob
 import logging
 import os
 import re
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Mapping, Optional, Union
@@ -186,15 +187,15 @@
                 target_schema_obj = mapper.derive_schema(transformer.specification)
                 if not target_schema_path.exists():
                     target_schema_path.parent.mkdir(exist_ok=True, parents=True)
                     yaml_dumper.dump(target_schema_obj, str(target_schema_path))
             for step in tr.steps:
                 input_obj = yaml.safe_load(open(str(root_directory / step.source_data)))
                 transformer.index(input_obj, step.source_class)
-                target_obj = transformer.transform(input_obj, source_type=step.source_class)
+                target_obj = transformer.map_object(input_obj, source_type=step.source_class)
                 if step.target_data:
                     out_path = output_directory / step.target_data
                     out_path.parent.mkdir(parents=True, exist_ok=True)
                     if out_path.exists():
                         line1 = open(str(out_path)).readline()
                         overwrite = "OVERWRITE" in line1
                         with open(str(out_path)) as f:
```

