# Comparing `tmp/cpr_sdk-1.0.2.tar.gz` & `tmp/cpr_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpr_sdk-1.0.2.tar", max compression
+gzip compressed data, was "cpr_sdk-1.1.0.tar", max compression
```

## Comparing `cpr_sdk-1.0.2.tar` & `cpr_sdk-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1507 2024-04-08 14:53:12.148240 cpr_sdk-1.0.2/LICENSE
--rw-r--r--   0        0        0     6615 2024-04-08 14:53:12.148240 cpr_sdk-1.0.2/README.md
--rw-r--r--   0        0        0     2885 2024-04-08 14:53:40.116331 cpr_sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       52 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/__init__.py
--rw-r--r--   0        0        0     5693 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/data_adaptors.py
--rw-r--r--   0        0        0     1118 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/embedding.py
--rw-r--r--   0        0        0      797 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/exceptions.py
--rw-r--r--   0        0        0    50630 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/models/__init__.py
--rw-r--r--   0        0        0    11979 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/models/search.py
--rw-r--r--   0        0        0    12721 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/parser_models.py
--rw-r--r--   0        0        0     2679 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/pipeline_general_models.py
--rw-r--r--   0        0        0    71013 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/resources/sensitive_query_terms.tsv
--rw-r--r--   0        0        0     2791 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/s3.py
--rw-r--r--   0        0        0     4584 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/search_adaptors.py
--rw-r--r--   0        0        0     4143 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/utils.py
--rw-r--r--   0        0        0      169 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/version.py
--rw-r--r--   0        0        0     6979 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/vespa.py
--rw-r--r--   0        0        0     7015 2024-04-08 14:53:12.152240 cpr_sdk-1.0.2/src/cpr_sdk/yql_builder.py
--rw-r--r--   0        0        0     7960 1970-01-01 00:00:00.000000 cpr_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6615 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0     2885 2024-04-11 09:15:35.217292 cpr_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/__init__.py
+-rw-r--r--   0        0        0     5693 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/data_adaptors.py
+-rw-r--r--   0        0        0     1118 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/embedding.py
+-rw-r--r--   0        0        0      797 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/exceptions.py
+-rw-r--r--   0        0        0    50630 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/models/__init__.py
+-rw-r--r--   0        0        0    11979 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/models/search.py
+-rw-r--r--   0        0        0    14816 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/parser_models.py
+-rw-r--r--   0        0        0     2679 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/pipeline_general_models.py
+-rw-r--r--   0        0        0    71013 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/resources/sensitive_query_terms.tsv
+-rw-r--r--   0        0        0     2791 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/s3.py
+-rw-r--r--   0        0        0     4584 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/search_adaptors.py
+-rw-r--r--   0        0        0     4143 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/utils.py
+-rw-r--r--   0        0        0      169 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/version.py
+-rw-r--r--   0        0        0     6979 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/vespa.py
+-rw-r--r--   0        0        0     7015 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/yql_builder.py
+-rw-r--r--   0        0        0     7960 1970-01-01 00:00:00.000000 cpr_sdk-1.1.0/PKG-INFO
```

### Comparing `cpr_sdk-1.0.2/LICENSE` & `cpr_sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/README.md` & `cpr_sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/pyproject.toml` & `cpr_sdk-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cpr_sdk"
 # This version in a placeholder and should not be updated. 
 # During the release flow the version from the cpr_sdk/__init__.py is used. 
-version = "1.0.2"
+version = "1.1.0"
 description = ""
 authors = ["CPR Tech <tech@climatepolicyradar.org>"]
 readme = "README.md"
 packages = [{include = "cpr_sdk", from = "src"}]
 classifiers = [
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
```

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/data_adaptors.py` & `cpr_sdk-1.1.0/src/cpr_sdk/data_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/embedding.py` & `cpr_sdk-1.1.0/src/cpr_sdk/embedding.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/exceptions.py` & `cpr_sdk-1.1.0/src/cpr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/models/__init__.py` & `cpr_sdk-1.1.0/src/cpr_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/models/search.py` & `cpr_sdk-1.1.0/src/cpr_sdk/models/search.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/parser_models.py` & `cpr_sdk-1.1.0/src/cpr_sdk/parser_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import logging.config
 from collections import Counter
 from datetime import date
 from enum import Enum
-from typing import List, Optional, Sequence, Tuple, TypeVar, Union
+import json
+from typing import List, Optional, Sequence, Tuple, TypeVar, Union, Any
 
 from cpr_sdk.pipeline_general_models import (
     CONTENT_TYPE_HTML,
     CONTENT_TYPE_PDF,
     BackendDocument,
     Json,
 )
@@ -369,7 +370,58 @@
         # We remove optional fields that have complex nested structures.
         # E.g. if html_data had a value of None for has_valid_text, we need to remove
         # it as this would throw a validation error.
         unflattened = remove_key_if_all_nested_vals_none(unflattened, "html_data")
         unflattened = remove_key_if_all_nested_vals_none(unflattened, "pdf_data")
 
         return ParserOutput.model_validate(unflattened)
+
+    def to_passage_level_json(self) -> list[dict[str, Any]]:
+        """
+        Convert the parser output to a passage-level JSON format.
+
+        In passage-level format we have a row for every text block in the document. This
+        is as for natural language processing tasks we often want to work with text at
+        the passage level.
+
+        HTML data won't contain PDF fields and vice versa, thus we must fill this in.
+        We could rely on the hugging face dataset transformation to fill in the missing
+        fields, but this is more explicit and provides default values.
+
+        The reason we convert from the pydantic BaseModel to a string using the
+        model_dump_json method and then reloading with json.load is as objects like
+        Enums and child pydantic objects persist when using the model_dump method.
+        We don't want these when we push to huggingface.
+        """
+        if self.text_blocks is None:
+            return []
+
+        common_fields_dict = json.loads(
+            self.model_dump_json(
+                exclude={
+                    "pdf_data": {"text_blocks", "page_metadata"},
+                    "html_data": {"text_blocks"},
+                }
+            )
+        )
+
+        passages_array = [
+            common_fields_dict
+            | json.loads(block.model_dump_json(exclude={"text"}))
+            | {"text": block.to_string(), "block_index": idx}
+            for idx, block in enumerate(self.text_blocks)
+        ]
+
+        empty_html_text_block_keys: list[str] = list(HTMLTextBlock.model_fields.keys())
+        empty_pdf_text_block_keys: list[str] = list(PDFTextBlock.model_fields.keys())
+
+        passages_array_filled = []
+        for passage in passages_array:
+            for key in empty_html_text_block_keys:
+                if key not in passage:
+                    passage[key] = None
+            for key in empty_pdf_text_block_keys:
+                if key not in passage:
+                    passage[key] = None
+            passages_array_filled.append(passage)
+
+        return passages_array_filled
```

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/pipeline_general_models.py` & `cpr_sdk-1.1.0/src/cpr_sdk/pipeline_general_models.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/resources/sensitive_query_terms.tsv` & `cpr_sdk-1.1.0/src/cpr_sdk/resources/sensitive_query_terms.tsv`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/s3.py` & `cpr_sdk-1.1.0/src/cpr_sdk/s3.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/search_adaptors.py` & `cpr_sdk-1.1.0/src/cpr_sdk/search_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/utils.py` & `cpr_sdk-1.1.0/src/cpr_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/vespa.py` & `cpr_sdk-1.1.0/src/cpr_sdk/vespa.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/src/cpr_sdk/yql_builder.py` & `cpr_sdk-1.1.0/src/cpr_sdk/yql_builder.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.0.2/PKG-INFO` & `cpr_sdk-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpr_sdk
-Version: 1.0.2
+Version: 1.1.0
 Summary: 
 License: LICENSE
 Author: CPR Tech
 Author-email: tech@climatepolicyradar.org
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

