# Comparing `tmp/cuckoo-hasura-0.1.6.tar.gz` & `tmp/cuckoo-hasura-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuckoo-hasura-0.1.6.tar", last modified: Tue Nov 28 22:27:10 2023, max compression
+gzip compressed data, was "cuckoo-hasura-0.1.7.tar", last modified: Thu Apr 11 16:38:47 2024, max compression
```

## Comparing `cuckoo-hasura-0.1.6.tar` & `cuckoo-hasura-0.1.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:27:10.597415 cuckoo-hasura-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2023-11-28 22:27:10.597415 cuckoo-hasura-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27567 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:27:10.593415 cuckoo-hasura-0.1.6/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/codegen/default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/codegen/example_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/codegen/graphql_2_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/codegen/model_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:27:10.593415 cuckoo-hasura-0.1.6/cuckoo/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/binary_tree_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18332 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/finalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/insert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:27:10.593415 cuckoo-hasura-0.1.6/cuckoo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/models/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/cuckoo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:27:10.597415 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2023-11-28 22:27:10.000000 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-11-28 22:27:10.000000 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 22:27:10.000000 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 22:27:10.000000 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-28 22:27:10.000000 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-28 22:27:10.000000 cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 22:27:10.597415 cuckoo-hasura-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:27:10.597415 cuckoo-hasura-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11125 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_include.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14426 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    29982 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    13266 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2023-11-28 22:27:04.000000 cuckoo-hasura-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27567 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.510962 cuckoo-hasura-0.1.7/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/example_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/graphql_2_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/model_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.514962 cuckoo-hasura-0.1.7/cuckoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/binary_tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/insert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.514962 cuckoo-hasura-0.1.7/cuckoo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_utils.py
```

### Comparing `cuckoo-hasura-0.1.6/LICENSE` & `cuckoo-hasura-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/PKG-INFO` & `cuckoo-hasura-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuckoo-hasura
-Version: 0.1.6
+Version: 0.1.7
 Summary: An easy to use GraphQL query builder, optimized for Hasura.
 Author-email: Kenta Fried <kenta.fried@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kenta Fried
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: orjson>=3.0.0
-Requires-Dist: pydantic>=1.0.0
+Requires-Dist: pydantic<2.0.0,>=1.0.0
 Requires-Dist: tenacity>=8.0.0
 Provides-Extra: codegen
 Requires-Dist: case-converter>=1.1.0; extra == "codegen"
 Requires-Dist: graphql-core>=3.2.3; extra == "codegen"
 
 # Cuckoo Hasura
```

### Comparing `cuckoo-hasura-0.1.6/README.md` & `cuckoo-hasura-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/codegen/default_config.py` & `cuckoo-hasura-0.1.7/codegen/default_config.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/codegen/example_config.py` & `cuckoo-hasura-0.1.7/codegen/example_config.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/codegen/graphql_2_python.py` & `cuckoo-hasura-0.1.7/codegen/graphql_2_python.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/codegen/model_module.py` & `cuckoo-hasura-0.1.7/codegen/model_module.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/cuckoo/binary_tree_node.py` & `cuckoo-hasura-0.1.7/cuckoo/binary_tree_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
+
+import inspect
+from pathlib import Path
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Optional,
     Type,
     TypeVar,
     Union,
-    TYPE_CHECKING,
 )
-import inspect
-from pathlib import Path
 
 from cuckoo.constants import ORDER_BY, WHERE
-from cuckoo.models import TMODEL
+from cuckoo.models import TMODEL, TableModel
 from cuckoo.utils import BracketStyle, in_brackets
 
 if TYPE_CHECKING:
-    from cuckoo.root_node import RootNode, HasuraClientError
-    from cuckoo.include import TCOLUMNS
     from cuckoo.finalizers import AggregatesDict, CountDict
+    from cuckoo.include import TCOLUMNS
+    from cuckoo.root_node import HasuraClientError, RootNode
 
 """The `BinaryTreeNode[TMODEL]` with its data class `GraphQLFragments`.
 
 The `BinaryTreeNode[TMODEL]` represents a node in a binary tree and it uses an instance
 of the `GraphQLFragments` class for storing its data. The `GraphQLFragments` data class
 contains a list of at least one response key class.
 """
@@ -231,18 +232,18 @@
 
     def __init__(
         self: BinaryTreeNode,
         model: Type[TMODEL],
         parent: Optional[BinaryTreeNode] = None,
     ):
         super().__init__()
-        self.model = model
+        self.model: Type[TMODEL] = model
         self._root: RootNode
-        self._parent: BinaryTreeNode
-        self._children: list[BinaryTreeNode] = []
+        self._parent: BinaryTreeNode[TableModel]
+        self._children: list[BinaryTreeNode[TableModel]] = []
         self._fragments = GraphQLFragments[TMODEL](self)
 
         if parent:
             self._bind_to_parent(parent)
             self._table_name = self._get_table_name_by_model()
             self._query_alias = self._root._generate_var_name()
         else:
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/constants.py` & `cuckoo-hasura-0.1.7/cuckoo/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from __future__ import annotations
+
 import os
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Literal,
     Type,
     TypedDict,
     Union,
-    TYPE_CHECKING,
 )
-from typing_extensions import TypeAlias, NotRequired
 
 from tenacity import stop_after_attempt, wait_random_exponential
+from typing_extensions import NotRequired, TypeAlias
 
 if TYPE_CHECKING:
-    from tenacity import (
-        StopBaseT,
-        WaitBaseT,
-        RetryBaseT,
-        RetryCallState,
-        RetryError,
-    )
+    from tenacity import RetryCallState, RetryError
+    from tenacity.retry import RetryBaseT
+    from tenacity.stop import StopBaseT
+    from tenacity.wait import WaitBaseT
 
+HASURA_PORT = int(os.environ.get("HASURA_PORT", "8080"))
+HASURA_HEALTH_URL = os.environ.get("HASURA_HEALTH_URL", "")
 HASURA_URL = os.environ["HASURA_URL"]
 HASURA_ADMIN_SECRET = os.environ["HASURA_ADMIN_SECRET"]
 HASURA_ROLE = os.environ["HASURA_ROLE"]
 
+DEFAULT_COLUMNS = ["uuid"]
+DEFAULT_COLUMNS_INVERTED = []
+
 
 class HasuraConfig(TypedDict):
     url: str
     headers: dict[str, str]
 
 
 class RetryConfig(TypedDict):
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/delete.py` & `cuckoo-hasura-0.1.7/cuckoo/delete.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/cuckoo/encoders.py` & `cuckoo-hasura-0.1.7/cuckoo/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 from pydantic import BaseModel
 from pydantic.json import ENCODERS_BY_TYPE
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
-def generate_encoders_by_class_tuples(
-    type_encoder_map: Dict[Any, Callable[[Any], Any]]
-) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
-    encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(
-        tuple
-    )
-    for type_, encoder in type_encoder_map.items():
-        encoders_by_class_tuples[encoder] += (type_,)
+def _generate_encoders_by_class_tuples(
+    type_encoder_map: Dict[type, Callable[[Any], Any]],
+) -> Dict[Callable[[Any], Any], Tuple[type]]:
+    encoders_by_class_tuples = defaultdict(tuple)
+    for type_to_encode, encoder in type_encoder_map.items():
+        encoders_by_class_tuples[encoder] += (type_to_encode,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
+encoders_by_class_tuples = _generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(
     obj: Any,
     include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
     exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
     by_alias: bool = True,
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/finalizers.py` & `cuckoo-hasura-0.1.7/cuckoo/finalizers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import annotations
+
 from typing import (
+    TYPE_CHECKING,
     Callable,
     Generator,
     Generic,
     Optional,
-    TypeVar,
     TypedDict,
+    TypeVar,
     Union,
-    TYPE_CHECKING,
 )
+
 from typing_extensions import NotRequired
 
 from cuckoo.binary_tree_node import (
     AffectedRowsResponseKey,
     AggregateResponseKey,
     BinaryTreeNode,
     ColumnResponseKey,
     NodesResponseKey,
     ReturningResponseKey,
 )
-from cuckoo.models.aggregate import TMODEL_BASE, TNUM_PROPS, Aggregate
-from cuckoo.models.common import TMODEL
+from cuckoo.constants import DEFAULT_COLUMNS, DEFAULT_COLUMNS_INVERTED
+from cuckoo.errors import HasuraClientError
+from cuckoo.models import TMODEL, TMODEL_BASE, TNUM_PROPS, Aggregate
 
 if TYPE_CHECKING:
-    from cuckoo.include import TINCLUDE, TCOLUMNS
+    from cuckoo.include import TCOLUMNS, TINCLUDE
 
 
 class CountDict(TypedDict):
     columns: NotRequired[set[str]]
     distinct: NotRequired[bool]
 
 
@@ -57,14 +60,33 @@
     def __init__(
         self,
         node: BinaryTreeNode,
     ):
         super().__init__()
         self._node: BinaryTreeNode = node
 
+    def _resolve_column_selection(
+        self,
+        columns: Optional[TCOLUMNS] = None,
+        invert_selection=False,
+    ):
+        if columns is None:
+            columns = DEFAULT_COLUMNS_INVERTED if invert_selection else DEFAULT_COLUMNS
+        if invert_selection:
+            field_names = {field_name for field_name, _, _ in self._node.model.fields()}
+            invalid_columns = list(filter(lambda col: col not in field_names, columns))
+            if invalid_columns:
+                raise HasuraClientError(
+                    "Invalid columns used with `invert_selection` option: "
+                    f"{invalid_columns}."
+                )
+            return field_names - set(columns)
+
+        return columns
+
 
 class ExecutingFinalizer(Finalizer):
     def __init__(
         self,
         node: BinaryTreeNode,
         **kwargs,
     ):
@@ -109,21 +131,29 @@
 
     async def _execute_async(self):
         if not self._node._root._is_batch:
             await self._node._root._execute_async()
 
 
 class AggregateBaseFinalizer(Finalizer):
-    def _validate_args(self, aggregates: AggregatesDict):
+    def _resolve_aggr_args(self, aggregates: AggregatesDict):
         if not any(aggregates.values()):
             raise ValueError(
                 "Missing argument. At least one argument is required: count, avg, max, "
                 "min, stddev, stddev_pop, stddev_samp, sum, var_pop, var_samp, "
                 "variance."
             )
+        return {
+            key: (
+                self._node._fragments.build_for_count(value)
+                if key == "count"
+                else value
+            )
+            for key, value in aggregates.items()
+        }
 
     def _to_aggr_dict(
         self,
         count: Optional[Union[bool, CountDict]] = None,
         avg: Optional[set[str]] = None,
         max: Optional[set[str]] = None,
         min: Optional[set[str]] = None,
@@ -149,24 +179,14 @@
                 ("var_pop", var_pop),
                 ("var_samp", var_samp),
                 ("variance", variance),
             ]
             if value is not None
         }
 
-    def _build_count_fragments(self, aggr: AggregatesDict):
-        return {
-            key: (
-                self._node._fragments.build_for_count(value)
-                if key == "count"
-                else value
-            )
-            for key, value in aggr.items()
-        }
-
 
 class YieldingFinalizer(
     ExecutingFinalizer,
     Generic[TYIELD],
 ):
     def __init__(
         self: YieldingFinalizer,
@@ -179,38 +199,48 @@
         super().__init__(node=node, **kwargs)
         self._returning_fn = returning_fn
         self._response_key = response_key
         self._gen_to_val = gen_to_val
 
     def yielding(
         self: YieldingFinalizer,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> Generator[TYIELD, None, None]:
-        self._node._fragments.response_keys.append(self._response_key(columns))
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
+        self._node._fragments.response_keys.append(self._response_key(resolved_columns))
         ExecutingFinalizer._bind_includes(self._node)
         self._execute()
 
         return self._returning_fn()
 
 
 class ReturningFinalizer(
     YieldingFinalizer[TYIELD],
     Generic[TYIELD, TRETURN],
 ):
     def returning(
         self: ReturningFinalizer,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> TRETURN:
-        return self._gen_to_val["returning"](super().yielding(columns))
+        return self._gen_to_val["returning"](
+            super().yielding(columns=columns, invert_selection=invert_selection)
+        )
 
     async def returning_async(
         self: ReturningFinalizer,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> TRETURN:
-        self._node._fragments.response_keys.append(self._response_key(columns))
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
+        self._node._fragments.response_keys.append(self._response_key(resolved_columns))
         ExecutingFinalizer._bind_includes(self._node)
         await self._execute_async()
 
         return self._gen_to_val["returning"](self._returning_fn())
 
 
 class YieldingAffectedRowsFinalizer(
@@ -240,18 +270,24 @@
         self._node._fragments.response_keys.append(AffectedRowsResponseKey())
         self._execute()
 
         return self._affected_rows_fn()
 
     def yielding_with_rows(
         self: YieldingAffectedRowsFinalizer,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> TYIELD_WITH:
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
         self._node._fragments.response_keys.extend(
-            [self._response_key(columns), AffectedRowsResponseKey()]
+            [
+                self._response_key(resolved_columns),
+                AffectedRowsResponseKey(),
+            ]
         )
         ExecutingFinalizer._bind_includes(self._node)
         self._execute()
 
         return self._returning_with_rows_fn()
 
 
@@ -269,26 +305,36 @@
         self._node._fragments.response_keys.append(AffectedRowsResponseKey())
         await self._execute_async()
 
         return self._gen_to_val["affected_rows"](self._affected_rows_fn())
 
     def returning_with_rows(
         self: AffectedRowsFinalizer,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> TRETURN_WITH:
         return self._gen_to_val["returning_with_rows"](
-            super().yielding_with_rows(columns=columns)
+            super().yielding_with_rows(
+                columns=columns, invert_selection=invert_selection
+            )
         )
 
     async def returning_with_rows_async(
         self: YieldingAffectedRowsFinalizer,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> TRETURN_WITH:
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
         self._node._fragments.response_keys.extend(
-            [self._response_key(columns), AffectedRowsResponseKey()]
+            [
+                self._response_key(resolved_columns),
+                AffectedRowsResponseKey(),
+            ]
         )
         ExecutingFinalizer._bind_includes(self._node)
         await self._execute_async()
 
         return self._gen_to_val["returning_with_rows"](self._returning_with_rows_fn())
 
 
@@ -311,14 +357,15 @@
             **kwargs,
         )
         self._aggregate_fn = aggregate_fn
         self._nodes_fn = nodes_fn
 
     def yield_on(
         self: YieldingAggregateFinalizer,
+        *,
         count: Optional[Union[bool, CountDict]] = None,
         avg: Optional[set[str]] = None,
         max: Optional[set[str]] = None,
         min: Optional[set[str]] = None,
         stddev: Optional[set[str]] = None,
         stddev_pop: Optional[set[str]] = None,
         stddev_samp: Optional[set[str]] = None,
@@ -336,48 +383,50 @@
             stddev_pop,
             stddev_samp,
             sum,
             var_pop,
             var_samp,
             variance,
         )
-        self._validate_args(aggregates)
+        resolved_aggregates = self._resolve_aggr_args(aggregates)
         self._node._fragments.response_keys.append(
-            AggregateResponseKey(aggregates=self._build_count_fragments(aggregates))
+            AggregateResponseKey(resolved_aggregates)
         )
         self._execute()
 
         return self._aggregate_fn()
 
     def yield_with_nodes(
         self: YieldingAggregateFinalizer,
         aggregates: AggregatesDict,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> tuple[Generator[Aggregate, None, None], Generator[TMODEL, None, None]]:
-        self._validate_args(aggregates)
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
+        resolved_aggregates = self._resolve_aggr_args(aggregates)
         self._node._fragments.response_keys.extend(
             [
-                AggregateResponseKey(
-                    aggregates=self._build_count_fragments(aggregates)
-                ),
-                NodesResponseKey(columns=columns),
+                AggregateResponseKey(resolved_aggregates),
+                NodesResponseKey(resolved_columns),
             ]
         )
         ExecutingFinalizer._bind_includes(self._node)
         self._execute()
 
         return (self._aggregate_fn(), self._nodes_fn())
 
 
 class AggregateFinalizer(
     YieldingAggregateFinalizer[TMODEL_BASE, TNUM_PROPS, TMODEL],
     Generic[TMODEL_BASE, TNUM_PROPS, TMODEL],
 ):
     def on(
         self,
+        *,
         count: Optional[Union[bool, CountDict]] = None,
         avg: Optional[set[str]] = None,
         max: Optional[set[str]] = None,
         min: Optional[set[str]] = None,
         stddev: Optional[set[str]] = None,
         stddev_pop: Optional[set[str]] = None,
         stddev_samp: Optional[set[str]] = None,
@@ -400,14 +449,15 @@
                 var_samp=var_samp,
                 variance=variance,
             )
         )
 
     async def on_async(
         self,
+        *,
         count: Optional[Union[bool, CountDict]] = None,
         avg: Optional[set[str]] = None,
         max: Optional[set[str]] = None,
         min: Optional[set[str]] = None,
         stddev: Optional[set[str]] = None,
         stddev_pop: Optional[set[str]] = None,
         stddev_samp: Optional[set[str]] = None,
@@ -425,45 +475,48 @@
             stddev_pop,
             stddev_samp,
             sum,
             var_pop,
             var_samp,
             variance,
         )
-        self._validate_args(aggregates)
+        resolved_aggregates = self._resolve_aggr_args(aggregates)
         self._node._fragments.response_keys.append(
-            AggregateResponseKey(aggregates=self._build_count_fragments(aggregates))
+            AggregateResponseKey(resolved_aggregates)
         )
         await self._execute_async()
 
         return next(self._aggregate_fn())
 
     def with_nodes(
         self,
         aggregates: AggregatesDict,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> tuple[Aggregate[TMODEL_BASE, TNUM_PROPS], list[TMODEL]]:
         aggregate_generator, nodes_generator = self.yield_with_nodes(
-            aggregates=aggregates, columns=columns
+            aggregates=aggregates, columns=columns, invert_selection=invert_selection
         )
 
         return (next(aggregate_generator), list(nodes_generator))
 
     async def with_nodes_async(
         self,
         aggregates: AggregatesDict,
-        columns: TCOLUMNS = ["uuid"],
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
     ) -> tuple[Aggregate[TMODEL_BASE, TNUM_PROPS], list[TMODEL]]:
-        self._validate_args(aggregates)
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
+        resolved_aggregates = self._resolve_aggr_args(aggregates)
         self._node._fragments.response_keys.extend(
             [
-                AggregateResponseKey(
-                    aggregates=self._build_count_fragments(aggregates)
-                ),
-                NodesResponseKey(columns=columns),
+                AggregateResponseKey(resolved_aggregates),
+                NodesResponseKey(resolved_columns),
             ]
         )
         ExecutingFinalizer._bind_includes(self._node)
         await self._execute_async()
 
         return (next(self._aggregate_fn()), list(self._nodes_fn()))
 
@@ -502,16 +555,22 @@
     ):
         super().__init__(
             node=node,
             **kwargs,
         )
         self._finalize_fn = finalize_fn
 
-    def returning(self, columns: TCOLUMNS = ["uuid"]):
-        self._node._fragments.response_keys.append(ColumnResponseKey(columns))
+    def returning(
+        self,
+        columns: Optional[TCOLUMNS] = None,
+        *,
+        invert_selection=False,
+    ):
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
+        self._node._fragments.response_keys.append(ColumnResponseKey(resolved_columns))
         return self._finalize_fn
 
 
 class AggregateIncludeFinalizer(AggregateBaseFinalizer):
     def __init__(
         self,
         node: BinaryTreeNode,
@@ -522,14 +581,15 @@
             node=node,
             **kwargs,
         )
         self._finalize_fn = finalize_fn
 
     def on(
         self,
+        *,
         count: Optional[Union[bool, CountDict]] = None,
         avg: Optional[set[str]] = None,
         max: Optional[set[str]] = None,
         min: Optional[set[str]] = None,
         stddev: Optional[set[str]] = None,
         stddev_pop: Optional[set[str]] = None,
         stddev_samp: Optional[set[str]] = None,
@@ -547,31 +607,34 @@
             stddev_pop,
             stddev_samp,
             sum,
             var_pop,
             var_samp,
             variance,
         )
-        self._validate_args(aggregates)
 
         def bind_and_configure(parent):
             include = self._finalize_fn(parent)
+            resolved_aggregates = self._resolve_aggr_args(aggregates)
             self._node._fragments.response_keys.append(
-                AggregateResponseKey(aggregates=self._build_count_fragments(aggregates))
+                AggregateResponseKey(resolved_aggregates)
             )
             return include
 
         return bind_and_configure
 
     def with_nodes(
         self,
         aggregates: AggregatesDict,
         columns: TCOLUMNS,
+        *,
+        invert_selection=False,
     ):
-        self._node._fragments.response_keys.append(NodesResponseKey(columns=columns))
+        resolved_columns = self._resolve_column_selection(columns, invert_selection)
+        self._node._fragments.response_keys.append(NodesResponseKey(resolved_columns))
 
         return self.on(**aggregates)
 
     def count(
         self,
         columns: Optional[set[str]] = None,
         distinct: Optional[bool] = None,
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/include.py` & `cuckoo-hasura-0.1.7/cuckoo/include.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 from __future__ import annotations
-from functools import reduce
+
 from typing import (
+    Any,
     Callable,
     Optional,
     Type,
     Union,
-    cast,
-    get_args,
-    get_origin,
 )
-from typing_extensions import TypeAlias
 
-from pydantic.fields import ModelField
+from typing_extensions import TypeAlias
 
 from cuckoo.binary_tree_node import BinaryTreeNode
 from cuckoo.constants import ORDER_BY, WHERE
 from cuckoo.errors import HasuraClientError
 from cuckoo.finalizers import (
     AggregateIncludeFinalizer,
     IncludeFinalizer,
 )
-from cuckoo.models import TMODEL, HasuraTableModel
+from cuckoo.models import TMODEL
 
 
 class Include(BinaryTreeNode[TMODEL]):
     def __init__(
         self,
         model: Type[TMODEL],
-        key: Optional[str] = None,
+        field_name: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(model=model, parent=None, **kwargs)
-        self._key = key
+        self._field_name = field_name
 
     def one(self):
         def bind_and_configure(parent: BinaryTreeNode):
             self._bind_to_parent(parent)
             self._fragments.query_name = self._get_relation_name()
             return self
 
@@ -83,65 +80,56 @@
                 offset=offset,
                 order_by=order_by,
             )
             return self
 
         return AggregateIncludeFinalizer(node=self, finalize_fn=bind_and_configure)
 
-    def _get_relation_name(self, is_list=False):
-        parent_model = cast(HasuraTableModel, self._parent.model)
-        if self._key is not None:
-            parent_key, model_of_key = next(
-                filter(
-                    lambda field: field[0] == self._key, parent_model.__fields__.items()
-                ),
-                (None, None),
-            )
-            if parent_key is None or model_of_key is None:
-                raise HasuraClientError(
-                    f"Invalid sub-query. The provided key `{self._key}` not found on "
-                    f"model `{parent_model}`"
-                )
-            elif model_of_key.type_ is not self.model:
-                raise HasuraClientError(
-                    f"Invalid sub-query. The provided model `{self.model}` "
-                    f"does not match expected model `{model_of_key.type_}`"
-                )
-            return parent_key
-
-        def find_model_attrs_by_type(
-            matching_keys: list[str], dict_items: tuple[str, ModelField]
-        ):
-            key, value = dict_items
-            if value.type_ is self.model:
-                if is_list:
-                    if get_origin(value.annotation) is Union and any(
-                        [get_origin(sub) is list for sub in get_args(value.annotation)]
-                    ):
-                        matching_keys.append(key)
-                else:
-                    matching_keys.append(key)
-            return matching_keys
-
-        matching_keys: list[str] = reduce(
-            find_model_attrs_by_type,
-            parent_model.__fields__.items(),
-            [],
-        )
+    def _get_relation_name(
+        self,
+        is_list=False,
+    ):
+        if self._field_name is not None:
+            self._verify_field_is_model(self._field_name)
+            return self._field_name
+
+        def match_model_type(field_info: tuple[str, Any, bool]):
+            (_, field_type, is_many_relation) = field_info
+            return field_type is self.model and is_list == is_many_relation
+
+        parent_field_names = [
+            field_name
+            for field_name, _, _ in filter(
+                match_model_type, self._parent.model.fields(include_relations=True)
+            )
+        ]
 
-        if len(matching_keys) == 0:
+        if len(parent_field_names) == 0:
             raise HasuraClientError(
                 "Invalid sub-query. Could not find any reference to "
                 + (f"List[{self.model}]" if is_list else f"{self.model}")
-                + f" in {parent_model}"
+                + f" in {self._parent.model}"
+            )
+        if len(parent_field_names) > 1:
+            raise HasuraClientError(
+                f"Ambiguous sub query. Candidates: {parent_field_names}. "
+                "Use the `field_name` argument to select one."
+            )
+
+        return parent_field_names.pop()
+
+    def _verify_field_is_model(self, field_name):
+        field_type = self._parent.model._get_field_type(field_name)
+        if field_type is None:
+            raise HasuraClientError(
+                f"Invalid sub-query. The provided `field_name={field_name}` does "
+                f"not exist on model `{self._parent.model}`."
             )
-        elif len(matching_keys) == 1:
-            return matching_keys[0]
-        else:
+        if field_type is not self.model:
             raise HasuraClientError(
-                f"Ambiguous sub query. Candidates: {matching_keys}. "
-                "Use the `key` argument to select one."
+                f"Invalid sub-query. The provided model `{self.model}` "
+                f"does not match expected model `{field_type}`."
             )
 
 
 TINCLUDE: TypeAlias = Callable[[BinaryTreeNode], Include]
 TCOLUMNS: TypeAlias = list[Union[str, TINCLUDE]]
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/insert.py` & `cuckoo-hasura-0.1.7/cuckoo/insert.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/cuckoo/mutation.py` & `cuckoo-hasura-0.1.7/cuckoo/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
+
 from contextlib import asynccontextmanager, contextmanager
 from logging import Logger
 from typing import Any, Generic, Optional, Type
 
 from httpx import AsyncClient, Client
 
 from cuckoo.binary_tree_node import BinaryTreeNode
 from cuckoo.constants import ORDER_BY, WHERE, CuckooConfig
 from cuckoo.errors import MutationFailedError
 from cuckoo.finalizers import (
-    ReturningFinalizer,
     TFIN_MANY,
     TFIN_ONE,
+    ReturningFinalizer,
     YieldingFinalizer,
 )
-from cuckoo.models import TMODEL
-from cuckoo.models.common import TBATCH_MODEL
+from cuckoo.models import TBATCH_MODEL, TMODEL
 from cuckoo.root_node import RootNode
 from cuckoo.utils import to_sql_function_args
 
 
 class InnerMutation(
     BinaryTreeNode[TMODEL],
     Generic[
@@ -188,17 +188,17 @@
             logger (Logger, optional): logger used internally. Defaults to None.
 
         Returns:
             Generator[tuple[type[Insert], type[Update], type[Delete]]]: the 3 mutation
             constructors. Any instance created by these is bound to the hasura
             transaction.
         """
+        from cuckoo.delete import BatchDelete
         from cuckoo.insert import BatchInsert
         from cuckoo.update import BatchUpdate
-        from cuckoo.delete import BatchDelete
 
         root = Mutation(
             model=object,  # hack
             config=config,
             session=session,
             logger=logger,
         )
@@ -235,17 +235,17 @@
     @staticmethod
     @asynccontextmanager
     async def batch_async(
         config: Optional[CuckooConfig] = None,
         session_async: Optional[AsyncClient] = None,
         logger: Optional[Logger] = None,
     ):
+        from cuckoo.delete import BatchDelete
         from cuckoo.insert import BatchInsert
         from cuckoo.update import BatchUpdate
-        from cuckoo.delete import BatchDelete
 
         root = Mutation(
             model=object,  # hack
             config=config,
             session_async=session_async,
             logger=logger,
         )
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/query.py` & `cuckoo-hasura-0.1.7/cuckoo/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 from __future__ import annotations
+
 from contextlib import asynccontextmanager, contextmanager
 from logging import Logger
 from typing import (
     Any,
     Generic,
     Optional,
     Type,
     cast,
 )
 from uuid import UUID
 
 from httpx import AsyncClient, Client
 
-from cuckoo.root_node import RootNode
 from cuckoo.binary_tree_node import BinaryTreeNode
 from cuckoo.constants import ORDER_BY, WHERE, CuckooConfig
 from cuckoo.errors import RecordNotFoundError
 from cuckoo.finalizers import (
-    AggregateFinalizer,
-    ReturningFinalizer,
     TFIN_AGGR,
     TFIN_MANY,
     TFIN_ONE,
+    AggregateFinalizer,
+    ReturningFinalizer,
     YieldingAggregateFinalizer,
     YieldingFinalizer,
 )
-from cuckoo.models import TMODEL, Aggregate
-from cuckoo.models.aggregate import (
+from cuckoo.models import (
+    TBATCH_MODEL,
     TBATCHMODEL_BASE,
     TBATCHNUM_PROPS,
+    TMODEL,
     TMODEL_BASE,
     TNUM_PROPS,
+    Aggregate,
+    UntypedModel,
 )
-from cuckoo.models.common import TBATCH_MODEL, UntypedModel
+from cuckoo.root_node import RootNode
 from cuckoo.utils import to_sql_function_args
 
 
 class InnerQuery(
     BinaryTreeNode[TMODEL],
     Generic[
         TMODEL,
         TFIN_ONE,
         TFIN_MANY,
         TFIN_AGGR,
         TMODEL_BASE,
         TNUM_PROPS,
     ],
 ):
-    """
-    The inner part of a query.
+    """The inner part of a query.
 
     Extends:
         - BinaryTreeNode: Provides properties and methods to create a binary tree.
     """
 
     def __init__(
         self,
@@ -92,28 +94,27 @@
         self._base_model = base_model
         self._numeric_model = numeric_model
 
     def one_by_pk(
         self,
         uuid: UUID,
     ):
-        """
-        Build a query for finding a single model by its UUID.
+        """Build a query for finding a single model by its UUID.
 
-        ### Args:
-        - `uuid`: The uuid of the record to query
+        Args:
+            uuid: The uuid of the record to query
 
-        ### Returns:
-        - `ReturningFinalizer[TMODEL]` for queries outside of a `batch()`
+        Returns:
+            ReturningFinalizer: if outside of a `batch()`
             execution context
-        - `YieldingFinalizer[TMODEL]` for queries inside a `batch()`
+            YieldingFinalizer: if inside a `batch()`
             execution context
 
-        ### Raises:
-        `NotFoundError` if no matching record was found
+        Raises:
+            NotFoundError: no matching record was found
         """
 
         inner_query = self._get_inner_query()
         var_name = self._root._generate_var_name()
         inner_query._fragments.query_name = (
             f"{inner_query._query_alias}: {inner_query._table_name}_by_pk"
         )
@@ -353,16 +354,15 @@
         ReturningFinalizer[TMODEL, TMODEL],
         ReturningFinalizer[TMODEL, list[TMODEL]],
         AggregateFinalizer[TMODEL_BASE, TNUM_PROPS, TMODEL],
         TMODEL_BASE,
         TNUM_PROPS,
     ],
 ):
-    """
-    Query builder for retrieving one, many, or an aggregate of models.
+    """Query builder for retrieving one, many, or an aggregate of models.
 
     Extends:
         RootNode: provides functionality to execute a query.
         InnerQuery: provides functionality to specify the kind of query to be created.
     """
 
     def __init__(
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/root_node.py` & `cuckoo-hasura-0.1.7/cuckoo/root_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
+
 from logging import Logger
 from types import GeneratorType
 from typing import (
     Any,
     Optional,
     Union,
 )
 
-from httpx import Client, Response, AsyncClient
 import orjson
+from httpx import AsyncClient, Client, Response
 from pydantic import BaseModel
-from tenacity import AsyncRetrying, Retrying, RetryError
+from tenacity import AsyncRetrying, RetryError, Retrying
 
 from cuckoo.binary_tree_node import BinaryTreeNode
 from cuckoo.constants import HASURA_DEFAULT_CONFIG, RETRY_DEFAULT_CONFIG, CuckooConfig
 from cuckoo.encoders import jsonable_encoder
 from cuckoo.errors import HasuraClientError, HasuraServerError
 from cuckoo.models import TMODEL
 from cuckoo.utils import in_brackets, to_truncated_str
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo/update.py` & `cuckoo-hasura-0.1.7/cuckoo/update.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/cuckoo/utils.py` & `cuckoo-hasura-0.1.7/cuckoo/utils.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/PKG-INFO` & `cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuckoo-hasura
-Version: 0.1.6
+Version: 0.1.7
 Summary: An easy to use GraphQL query builder, optimized for Hasura.
 Author-email: Kenta Fried <kenta.fried@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kenta Fried
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: orjson>=3.0.0
-Requires-Dist: pydantic>=1.0.0
+Requires-Dist: pydantic<2.0.0,>=1.0.0
 Requires-Dist: tenacity>=8.0.0
 Provides-Extra: codegen
 Requires-Dist: case-converter>=1.1.0; extra == "codegen"
 Requires-Dist: graphql-core>=3.2.3; extra == "codegen"
 
 # Cuckoo Hasura
```

### Comparing `cuckoo-hasura-0.1.6/cuckoo_hasura.egg-info/SOURCES.txt` & `cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 cuckoo/insert.py
 cuckoo/mutation.py
 cuckoo/query.py
 cuckoo/root_node.py
 cuckoo/update.py
 cuckoo/utils.py
 cuckoo/models/__init__.py
-cuckoo/models/aggregate.py
+cuckoo/models/builtins.py
 cuckoo/models/common.py
+cuckoo/models/providers.py
 cuckoo_hasura.egg-info/PKG-INFO
 cuckoo_hasura.egg-info/SOURCES.txt
 cuckoo_hasura.egg-info/dependency_links.txt
 cuckoo_hasura.egg-info/entry_points.txt
 cuckoo_hasura.egg-info/requires.txt
 cuckoo_hasura.egg-info/top_level.txt
 tests/test_delete.py
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_delete.py` & `cuckoo-hasura-0.1.7/tests/test_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 from httpx import AsyncClient, Client
 from pytest import fixture, mark, raises
 
 from cuckoo import Delete, Query
 from cuckoo.errors import RecordNotFoundError
 from tests.fixture.common_fixture import (
     ARTICLE_COMMENT_CONDITIONALS,
-    FinalizeReturning,
     FinalizeParams,
+    FinalizeReturning,
 )
 from tests.fixture.common_utils import (
     all_columns,
+    assert_authors_ordered,
     delete_all,
     persist_authors,
-    assert_authors_ordered,
 )
 from tests.fixture.query_fixture import AUTHOR_ARTICLE_COMMENT_CONDITIONALS
 from tests.fixture.sample_models import Author
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Delete).returning_one())
 class TestOneByPK:
     async def test_deleting_a_model_if_record_exists(
         self,
         finalize: FinalizeReturning[Delete, Author],
         persisted_authors: list[Author],
         session: Client,
@@ -110,14 +111,15 @@
             session=session,
             session_async=session_async,
         )
 
         assert actual_author.uuid == existing_uuid
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Delete).returning_many())
 class TestMany:
     async def test_returning_an_empty_list_if_non_matching_condition_is_provided(
         self,
         finalize: FinalizeReturning[Delete, list[Author]],
         session: Client,
         session_async: AsyncClient,
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_include.py` & `cuckoo-hasura-0.1.7/tests/test_include.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+import re
 from typing import Callable
 from uuid import UUID
+
 from httpx import AsyncClient, Client
-from pytest import fixture, raises, mark
+from pytest import fixture, mark, raises
 
 from cuckoo import Include, Query
 from cuckoo.delete import Delete
 from cuckoo.errors import HasuraClientError
-from cuckoo.models.aggregate import Aggregate
+from cuckoo.models import Aggregate
 from tests.fixture.common_fixture import (
     FinalizeParams,
     FinalizeReturning,
 )
 from tests.fixture.common_utils import (
     persist_author_details,
     persist_authors,
 )
 from tests.fixture.include_fixture import (
     ARTICLE_AGGREGATES,
     ARTICLE_CONDITIONALS,
     SUGAR_FUNCTIONS,
 )
 from tests.fixture.sample_models.public import (
-    AuthorDetail,
-    Comment,
     Address,
-    Author,
     Article,
+    Author,
+    AuthorDetail,
+    Comment,
 )
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_one())
 class TestOne:
     async def test_can_include_by_key_for_model_with_ambiguous_submodels(
         self,
         finalize: FinalizeReturning[Query, AuthorDetail],
         persisted_detail: AuthorDetail,
         session: Client,
@@ -41,27 +44,27 @@
         detail_prim = await finalize(
             run_test=lambda Query: Query(AuthorDetail).one_by_pk(
                 uuid=persisted_detail.uuid
             ),
             session=session,
             session_async=session_async,
             columns=[
-                Include(Address, key="primary_address")
+                Include(Address, field_name="primary_address")
                 .one()
                 .returning(columns=["street"])
             ],
         )
         detail_sec = await finalize(
             run_test=lambda Query: Query(AuthorDetail).one_by_pk(
                 uuid=persisted_detail.uuid
             ),
             session=session,
             session_async=session_async,
             columns=[
-                Include(Address, key="secondary_address")
+                Include(Address, field_name="secondary_address")
                 .one()
                 .returning(columns=["street"])
             ],
         )
 
         assert detail_prim.primary_address.street == "primary street"
         assert detail_prim.secondary_address is None
@@ -78,19 +81,20 @@
         with raises(HasuraClientError) as err:
             await finalize(
                 run_test=lambda Query: Query(AuthorDetail).one_by_pk(
                     uuid=persisted_detail.uuid
                 ),
                 session=session,
                 session_async=session_async,
-                columns=[Include(Address, key="INVALID").one().returning()],
+                columns=[Include(Address, field_name="INVALID").one().returning()],
             )
 
         assert (
-            "Invalid sub-query. The provided key `INVALID` not found on model "
+            "Invalid sub-query. "
+            "The provided `field_name=INVALID` does not exist on model "
             "`<class 'tests.fixture.sample_models.public.author_detail.AuthorDetail'>`"
         ) in str(err)
 
     async def test_raises_client_error_if_key_to_include_exists_but_model_does_not_match_key(
         self,
         finalize: FinalizeReturning[Query, AuthorDetail],
         persisted_detail: AuthorDetail,
@@ -100,15 +104,17 @@
         with raises(HasuraClientError) as err:
             await finalize(
                 run_test=lambda Query: Query(AuthorDetail).one_by_pk(
                     uuid=persisted_detail.uuid
                 ),
                 session=session,
                 session_async=session_async,
-                columns=[Include(Comment, key="primary_address").one().returning()],
+                columns=[
+                    Include(Comment, field_name="primary_address").one().returning()
+                ],
             )
 
         assert (
             "Invalid sub-query. The provided model "
             "`<class 'tests.fixture.sample_models.public.comment.Comment'>` does not "
             "match expected model "
             "`<class 'tests.fixture.sample_models.public.address.Address'>`"
@@ -150,19 +156,22 @@
                     uuid=persisted_detail.uuid
                 ),
                 session=session,
                 session_async=session_async,
                 columns=[Include(Address).one().returning()],
             )
 
-        assert (
-            "Ambiguous sub query. "
-            "Candidates: ['primary_address', 'secondary_address']. "
-            "Use the `key` argument to select one."
-        ) in str(err)
+        match = re.match(
+            r".*Ambiguous sub query. Candidates: \['(\w+)', '(\w+)'\]\. "
+            r"Use the `field_name` argument to select one\.",
+            str(err),
+        )
+        assert match
+        field_names = match.groups()
+        assert set(field_names) == {"primary_address", "secondary_address"}
 
     async def test_raises_error_if_including_invalid_object(
         self,
         finalize: FinalizeReturning[Query, AuthorDetail],
         persisted_detail: AuthorDetail,
         session: Client,
         session_async: AsyncClient,
@@ -179,14 +188,15 @@
 
         assert (
             "Elements in `returning` need to be of type `str` or an instance of `Include`. "
             "Found type=<class 'cuckoo.finalizers.IncludeFinalizer'>."
         ) in str(err)
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_one())
 class TestAggregate:
     @mark.parametrize(**ARTICLE_AGGREGATES)
     async def test_aggregate_on_without_conditions(
         self,
         finalize: FinalizeReturning[Query, Author],
         persisted_author: Author,
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_insert.py` & `cuckoo-hasura-0.1.7/tests/test_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import Callable
 from uuid import UUID
 
 from httpx import AsyncClient, Client
-from pytest import mark, fixture, raises
+from pytest import fixture, mark, raises
 
-from cuckoo import Query, Insert, Delete
+from cuckoo import Delete, Insert, Query
 from cuckoo.errors import InsertFailedError
-from tests.fixture.insert_fixture import (
-    INPUT_DATA,
-    INPUT_DATA_LIST,
-    COLUMNS_ARG,
-)
 from tests.fixture.common_fixture import (
     FinalizeAffectedRows,
-    FinalizeReturning,
     FinalizeParams,
+    FinalizeReturning,
+)
+from tests.fixture.insert_fixture import (
+    COLUMNS_ARG,
+    INPUT_DATA,
+    INPUT_DATA_LIST,
 )
 from tests.fixture.sample_models.public import Author
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Insert).returning_one())
 class TestInsertOne:
     @mark.parametrize(**COLUMNS_ARG)
     @mark.parametrize(**INPUT_DATA)
     async def test_inserting_data(
         self,
         finalize: FinalizeReturning[Insert, Author],
@@ -157,14 +158,15 @@
                 ),
                 columns=["uuid", "name"],
                 session=session,
                 session_async=session_async,
             )
 
 
+@mark.asyncio(scope="session")
 class TestInsertMany:
     @mark.parametrize(**FinalizeParams(Insert).returning_many())
     @mark.parametrize(**COLUMNS_ARG)
     @mark.parametrize(**INPUT_DATA_LIST)
     async def test_returning_all_fields_and_relations_with_conditions(
         self,
         finalize: FinalizeReturning[Insert, list[Author]],
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_mutation.py` & `cuckoo-hasura-0.1.7/tests/test_mutation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
 from typing import Any, Callable, Type
+from unittest.mock import ANY
 from uuid import UUID, uuid4
-from geojson_pydantic import Point, Polygon
 
+from geojson_pydantic import Polygon
 from httpx import AsyncClient, Client
 from pytest import fixture, mark, raises
 
 from cuckoo import Mutation, Query
 from cuckoo.delete import BatchDelete
 from cuckoo.errors import HasuraClientError
 from cuckoo.insert import BatchInsert
 from cuckoo.update import BatchUpdate
-
 from tests.fixture.common_fixture import (
     ARTICLE_COMMENT_CONDITIONALS,
     FinalizeParams,
     FinalizeReturning,
 )
 from tests.fixture.common_utils import (
     all_columns,
@@ -26,18 +26,19 @@
 from tests.fixture.mutation_fixture import MUTATIONS1, MUTATIONS2
 from tests.fixture.query_fixture import (
     AUTHOR_ARTICLE_COMMENT_CONDITIONALS,
 )
 from tests.fixture.sample_models import Author
 
 
+@mark.asyncio(scope="session")
 class TestBatch:
     @mark.parametrize(**MUTATIONS1)
     @mark.parametrize(**MUTATIONS2)
-    def test_two_mutations_in_batch(
+    async def test_two_mutations_in_batch(
         self,
         persisted_authors: list[Author],
         run_and_assert1: Callable[
             [list[Author], Client],
             tuple[
                 Callable[
                     [Type[BatchInsert], Type[BatchUpdate], Type[BatchDelete], UUID], Any
@@ -130,15 +131,15 @@
                 BatchDelete,
                 user_uuid,
             )
 
         assert_model1(actual1)
         assert_model2(actual2)
 
-    def test_raises_client_error_when_trying_to_access_result_of_unexecuted_batch(
+    async def test_raises_client_error_when_trying_to_access_result_of_unexecuted_batch(
         self,
         session: Client,
     ):
         with raises(HasuraClientError) as err:
             with Mutation.batch(session=session) as (_, _, BatchDelete, _):
                 actual1 = BatchDelete(Author).many(where={}).yielding()
 
@@ -146,14 +147,15 @@
 
         assert (
             "Cannot access response data before calling `RootNode._make_request`"
             in str(err)
         )
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Mutation).returning_one())
 class TestOneFunction:
     async def test_mutating_one_record_with_provided_arg_matching_record(
         self,
         finalize: FinalizeReturning[Mutation, Author],
         persisted_authors: list[Author],
         session: Client,
@@ -301,36 +303,40 @@
         get_article_conditional: Callable[[Author], dict[str, Any]],
         get_comment_conditional: Callable[[Author], dict[str, Any]],
         get_expected_author: Callable[[Author], Author],
         session: Client,
         session_async: AsyncClient,
     ):
         random_author = persisted_authors[7]
+        user_uuid = uuid4()
         expected_author = get_expected_author(random_author)
         expected_author.age += 1
+        expected_author.updated_by = user_uuid
+        expected_author.updated_at = ANY
 
         actual_author = await finalize(
             run_test=lambda Mutation: Mutation(Author).one_function(
                 "inc_author_age",
                 args={
                     "author_uuid": random_author.uuid,
-                    "user_uuid": uuid4(),
+                    "user_uuid": user_uuid,
                 },
             ),
             columns=all_columns(
                 article_args=get_article_conditional(random_author),
                 comment_args=get_comment_conditional(random_author),
             ),
             session=session,
             session_async=session_async,
         )
 
         assert_authors_ordered([actual_author], [expected_author])
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Mutation).returning_many())
 class TestManyFunction:
     async def test_mutating_records_with_provided_arg_matching_records(
         self,
         finalize: FinalizeReturning[Mutation, list[Author]],
         persisted_authors: list[Author],
         session: Client,
@@ -402,25 +408,32 @@
         get_article_conditional: Callable[[list[Author]], dict[str, Any]],
         get_comment_conditional: Callable[[list[Author]], dict[str, Any]],
         get_expected_authors: Callable[[list[Author]], list[Author]],
         assert_authors: Callable[[list[Author], list[Author]], None],
         session: Client,
         session_async: AsyncClient,
     ):
+        user_uuid = uuid4()
         expected_authors = [
-            author.copy(update={"age": author.age + 1})
+            author.copy(
+                update={
+                    "age": author.age + 1,
+                    "updated_by": user_uuid,
+                    "updated_at": ANY,
+                }
+            )
             for author in get_expected_authors(persisted_authors)
         ]
 
         actual_authors = await finalize(
             run_test=lambda Mutation: Mutation(Author).many_function(
                 "inc_all_authors_age",
                 args={
                     "author_uuids": [author.uuid for author in persisted_authors],
-                    "user_uuid": uuid4(),
+                    "user_uuid": user_uuid,
                 },
                 **get_author_condition(persisted_authors),
             ),
             columns=all_columns(
                 article_args=get_article_conditional(persisted_authors),
                 comment_args=get_comment_conditional(persisted_authors),
             ),
@@ -433,12 +446,12 @@
 
 @fixture
 def persisted_authors(user_uuid: UUID, session: Client, session_async: AsyncClient):
     delete_all(session=session)
     return persist_authors(
         user_uuid,
         num_authors=20,
-        # Note that update and delete tests use `authors.pop()` to "reserve" their own
-        # test record
+        # Note that update and delete tests use `authors.pop()` to prevent
+        # interdependent test cases
         session=session,
         session_async=session_async,
     )
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_query.py` & `cuckoo-hasura-0.1.7/tests/test_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,53 @@
+import asyncio
 import logging
+from datetime import datetime
 from logging import LogRecord
 from typing import Any, Callable, Iterable, cast
 from uuid import UUID, uuid4
-from httpx import AsyncClient, Client
 
-from pytest import fixture, mark, raises, LogCaptureFixture
+from httpx import AsyncClient, Client
+from pytest import LogCaptureFixture, fixture, mark, raises
 
-from cuckoo import Query
-from cuckoo.errors import HasuraServerError, RecordNotFoundError
-from cuckoo.models.aggregate import Aggregate, AggregateResponse
+from cuckoo import TCOLUMNS, Insert, Query
+from cuckoo.errors import HasuraClientError, HasuraServerError, RecordNotFoundError
+from cuckoo.include import Include
+from cuckoo.models import Aggregate, AggregateResponse
 from tests.fixture.common_fixture import (
     ARTICLE_COMMENT_CONDITIONALS,
+    AUTHOR_RELATIONS,
+    FinalizeAggregate,
     FinalizeParams,
     FinalizeReturning,
-    FinalizeAggregate,
     FinalizeWithNodes,
 )
 from tests.fixture.common_utils import (
     DEFAULT_COUNTS,
     all_columns,
+    assert_authors_ordered,
     delete_all,
     persist_authors,
-    assert_authors_ordered,
 )
 from tests.fixture.query_fixture import (
     AUTHOR_AGGREGATES,
     AUTHOR_ARTICLE_COMMENT_CONDITIONALS,
     AUTHOR_CONDITIONALS,
     SUGAR_FUNCTIONS,
 )
-from tests.fixture.sample_models.public.author import Author, AuthorBase, AuthorNumerics
-from tests.fixture.sample_models.public.article import Article
-from tests.fixture.sample_models.public.comment import Comment
+from tests.fixture.sample_models.public import (
+    Article,
+    Author,
+    AuthorBase,
+    AuthorDetail,
+    AuthorNumerics,
+    Comment,
+)
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_one())
 class TestOneByPK:
     async def test_finding_a_model_if_record_exists(
         self,
         finalize: FinalizeReturning[Query, Author],
         persisted_authors: list[Author],
         session: Client,
@@ -93,14 +103,116 @@
             ),
             session=session,
             session_async=session_async,
         )
 
         assert_authors_ordered([actual_author], [expected_author])
 
+    @mark.parametrize(
+        argnames=["get_columns", "invert_selection", "get_expected_author"],
+        argvalues=[
+            (
+                lambda: None,
+                False,
+                lambda author: author.copy(include={"uuid"}),
+            ),
+            (
+                lambda: ["name"],
+                False,
+                lambda author: author.copy(include={"name"}),
+            ),
+            (
+                lambda: ["name"],
+                True,
+                lambda author: author.copy(exclude={"name", *AUTHOR_RELATIONS}),
+            ),
+            (
+                lambda: [],
+                True,
+                lambda author: author.copy(exclude=AUTHOR_RELATIONS),
+            ),
+            (
+                lambda: None,
+                True,
+                lambda author: author.copy(exclude=AUTHOR_RELATIONS),
+            ),
+            (
+                lambda: [Include(AuthorDetail).one().returning(invert_selection=True)],
+                False,
+                lambda author: author.copy(include={"detail"}),
+            ),
+        ],
+        ids=[
+            "default column",
+            "one column",
+            "all but one column",
+            "all columns, empty selection",
+            "all columns, no selection",
+            "all columns of included relation",
+        ],
+    )
+    async def test_returning_columns(
+        self,
+        finalize: FinalizeReturning[Query, Author],
+        persisted_authors: list[Author],
+        get_columns: Callable[[], TCOLUMNS],
+        invert_selection: bool,
+        get_expected_author: Callable[[Author], Author],
+        session: Client,
+        session_async: AsyncClient,
+    ):
+        some_author = persisted_authors[7]
+        expected = get_expected_author(some_author)
+
+        actual = await finalize(
+            run_test=lambda Query: Query(Author).one_by_pk(uuid=some_author.uuid),
+            columns=get_columns(),
+            invert_selection=invert_selection,
+            session=session,
+            session_async=session_async,
+        )
+
+        assert_authors_ordered([actual], [expected])
+
+    @mark.parametrize(
+        argnames=["columns"],
+        argvalues=[
+            (["non_existing_column"],),
+            ([Include(Article).many().returning()],),
+            (["articles { uuid }"],),
+            ([None],),
+        ],
+        ids=[
+            "non-existing column",
+            "Include",
+            "relation as a string",
+            "None",
+        ],
+    )
+    async def test_raises_error_if_column_selection_is_inverted_with_invalid_columns(
+        self,
+        finalize: FinalizeReturning[Query, Author],
+        persisted_authors: list[Author],
+        columns: TCOLUMNS,
+        session: Client,
+        session_async: AsyncClient,
+    ):
+        some_author = persisted_authors[3]
+
+        with raises(HasuraClientError) as err:
+            await finalize(
+                run_test=lambda Query: Query(Author).one_by_pk(uuid=some_author.uuid),
+                columns=columns,
+                invert_selection=True,
+                session=session,
+                session_async=session_async,
+            )
+
+        assert "Invalid columns used with `invert_selection` option: " in str(err.value)
+
     async def test_successful_query_gets_logged(
         self,
         finalize: FinalizeReturning[Query, Author],
         persisted_authors: list[Author],
         caplog: LogCaptureFixture,
         session: Client,
         session_async: AsyncClient,
@@ -167,14 +279,15 @@
         )
         assert record
         assert "authors_by_pk" in record.msg
         assert str(existing_uuid) in record.msg
         assert "field 'does_not_exist' not found in type: 'authors'" in record.msg
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_many())
 class TestMany:
     async def test_finding_all_records_with_default_column_if_no_condition_is_provided(
         self,
         finalize: FinalizeReturning[Query, list[Author]],
         persisted_authors: list[Author],
         session: Client,
@@ -251,14 +364,58 @@
             session=session,
             session_async=session_async,
         )
 
         assert_authors(actual_authors, expected_authors)
 
 
+@mark.asyncio(scope="session")
+class TestManyYielding:
+    @mark.performance
+    @mark.slow
+    async def test_memory_consumption_is_below_threshold(
+        self,
+        session: Client,
+        session_async: AsyncClient,
+    ):
+        BATCH_SIZE = 10000
+        CONCURRENCY = 4
+        for _ in range(100):
+            await asyncio.gather(
+                *(
+                    [
+                        Insert(Author, session_async=session_async)
+                        .many(
+                            data=(
+                                [
+                                    {
+                                        "name": "one of a million",
+                                        "created_by": uuid4(),
+                                        "updated_by": uuid4(),
+                                    }
+                                ]
+                                * BATCH_SIZE
+                            )
+                        )
+                        .returning_async()
+                    ]
+                    * CONCURRENCY
+                )
+            )
+
+        print("START ", datetime.now().isoformat())
+        count = 0
+        # for author in await Query(Author).many(where={}).returning_async():
+        for author in Query(Author).many(where={}).yielding():
+            # assert isinstance(author.uuid, UUID)
+            count += 1
+        print("END ", count, datetime.now().isoformat())
+
+
+@mark.asyncio(scope="session")
 class TestAggregate:
     @mark.parametrize(**FinalizeParams(Query).aggregate())
     @mark.parametrize(**AUTHOR_AGGREGATES)
     async def test_aggregate_on_without_conditions(
         self,
         finalize: FinalizeAggregate[AuthorBase, AuthorNumerics, Author],
         aggregate_arg: dict,
@@ -377,14 +534,15 @@
             Query(Author, session=session, session_async=session_async).aggregate(),
             fn_name,
         )(**args)
 
         assert get_value(actual) == expected
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_one())
 class TestOneFunction:
     async def test_finding_one_record_with_default_arg_matching_record(
         self,
         finalize: FinalizeReturning[Query, Author],
         persisted_authors: list[Author],
         session: Client,
@@ -468,14 +626,15 @@
             session=session,
             session_async=session_async,
         )
 
         assert_authors_ordered([actual_author], [expected_author])
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_many())
 class TestManyFunction:
     async def test_finding_all_records_with_default_arg_matching_records(
         self,
         finalize: FinalizeReturning[Query, list[Author]],
         persisted_authors: list[Author],
         session: Client,
@@ -561,14 +720,15 @@
             session=session,
             session_async=session_async,
         )
 
         assert_authors(actual_authors, expected_authors)
 
 
+@mark.asyncio(scope="session")
 class TestAggregateFunction:
     @mark.parametrize(**FinalizeParams(Query).aggregate())
     @mark.parametrize(**AUTHOR_AGGREGATES)
     async def test_aggregate_on_without_conditions(
         self,
         finalize: FinalizeAggregate[AuthorBase, AuthorNumerics, Author],
         aggregate_arg: dict,
@@ -701,14 +861,15 @@
             ),
             fn_name,
         )(**args)
 
         assert get_value(actual) == expected
 
 
+@mark.asyncio(scope="session")
 class TestBatch:
     async def test_mixing_multiple_queries(
         self,
         persisted_authors: list[Author],
         session: Client,
         session_async: AsyncClient,
     ):
@@ -805,15 +966,15 @@
                 with raises(AttributeError):
                     BatchQuery(Author).aggregate().on()
 
                 with raises(AttributeError):
                     BatchQuery(Author).aggregate().with_nodes()
 
 
-@fixture(scope="module", autouse=True)
+@fixture(scope="module")
 def persisted_authors(user_uuid: UUID, session: Client, session_async: AsyncClient):
     delete_all(session=session)
 
     return persist_authors(user_uuid, session=session, session_async=session_async)
 
 
 @fixture(scope="module")
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_root_node.py` & `cuckoo-hasura-0.1.7/tests/test_root_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+import time
 from statistics import mean
 from typing import Any, Callable, Type
 from unittest.mock import MagicMock, patch
 from uuid import uuid4
-import time
-from httpx import AsyncClient, Client
 
-from pytest import mark, fixture, raises
+from httpx import AsyncClient, Client
+from pytest import fixture, mark, raises
 from tenacity import stop_after_attempt
 
-from cuckoo import Query
-from cuckoo import root_node
+from cuckoo import Query, root_node
 from cuckoo.errors import HasuraServerError
 from cuckoo.include import Include
 from tests.fixture.base_fixture import VARIABLE_SEQUENCES, VARIABLE_TYPES
 from tests.fixture.common_utils import generate_author_data
 from tests.fixture.sample_models.public import Article, Author
 
 
@@ -226,40 +225,47 @@
             root_node.Client,
             "close",
             wraps=root_node.Client().close,
         ) as spy:
             yield spy
 
 
+@mark.asyncio(scope="session")
 class TestExecuteAsync:
     async def test_default_config_stops_retrying_after_5_attempts(
         self,
         failing_session: MagicMock,
     ):
         with raises(HasuraServerError):
-            await Query(Author, session_async=failing_session).many(
-                where={}
-            ).returning_async()
+            await (
+                Query(Author, session_async=failing_session)
+                .many(where={})
+                .returning_async()
+            )
 
         assert failing_session.post.call_count == 5
 
     async def test_retry_config_can_be_changed(
         self,
         failing_session: MagicMock,
     ):
         with raises(HasuraServerError):
-            await Query(
-                Author,
-                session_async=failing_session,
-                config={
-                    "retry": {
-                        "stop": stop_after_attempt(3),
-                    }
-                },
-            ).many(where={}).returning_async()
+            await (
+                Query(
+                    Author,
+                    session_async=failing_session,
+                    config={
+                        "retry": {
+                            "stop": stop_after_attempt(3),
+                        }
+                    },
+                )
+                .many(where={})
+                .returning_async()
+            )
 
         assert failing_session.post.call_count == 3
 
     async def test_default_session_gets_closed_for_successful_query(
         self,
         default_session_close: MagicMock,
     ):
@@ -276,28 +282,30 @@
 
         failing_default_session.aclose.assert_called_once()
 
     async def test_non_default_session_does_not_get_closed_for_successful_query(
         self,
         session_async: AsyncClient,
     ):
-        await Query(Author, session_async=session_async).many(
-            where={}
-        ).returning_async()
+        await (
+            Query(Author, session_async=session_async).many(where={}).returning_async()
+        )
 
         assert not session_async.is_closed
 
     async def test_non_default_session_does_not_get_closed_for_unsuccessful_query(
         self,
         failing_session: MagicMock,
     ):
         with raises(HasuraServerError):
-            await Query(Author, session_async=failing_session).many(
-                where={}
-            ).returning_async()
+            await (
+                Query(Author, session_async=failing_session)
+                .many(where={})
+                .returning_async()
+            )
 
         failing_session.aclose.assert_not_called()
 
     @fixture
     def failing_session(self):
         mock = MagicMock(spec=AsyncClient)
         mock.post.side_effect = [
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_update.py` & `cuckoo-hasura-0.1.7/tests/test_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from typing import Any, Callable
 from uuid import UUID, uuid4
-from httpx import AsyncClient, Client
 
+from httpx import AsyncClient, Client
 from pytest import fixture, mark, raises
 
-from cuckoo import Update, Include
+from cuckoo import Update
 from cuckoo.errors import RecordNotFoundError
+from tests.fixture.common_fixture import (
+    ARTICLE_COMMENT_CONDITIONALS,
+    FinalizeAffectedRows,
+    FinalizeParams,
+    FinalizeReturning,
+)
 from tests.fixture.common_utils import (
     all_columns,
     assert_authors_ordered,
     assert_authors_unordered,
     delete_all,
     persist_authors,
 )
-from tests.fixture.common_fixture import (
-    ARTICLE_COMMENT_CONDITIONALS,
-    FinalizeAffectedRows,
-    FinalizeReturning,
-    FinalizeParams,
-)
+from tests.fixture.sample_models import Author
 from tests.fixture.update_fixture import (
     AUTHOR_ARTICLE_COMMENT_CONDITIONALS,
-    UPDATE_DISTINCT_ARGS,
     UPDATE_ARGS,
+    UPDATE_DISTINCT_ARGS,
 )
-from tests.fixture.sample_models import Author, AuthorDetail, Comment, Article
 
 
+@mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Update).returning_one())
 class TestOneByPK:
     @mark.parametrize(**UPDATE_ARGS)
     async def test_updating_an_existing_model(
         self,
         finalize: FinalizeReturning[Update, Author],
         persisted_authors: list[Author],
@@ -113,30 +114,36 @@
         get_comment_conditional: Callable[[Author], dict[str, Any]],
         get_expected_author: Callable[[Author], Author],
         session: Client,
         session_async: AsyncClient,
     ):
         some_author = persisted_authors[0]
         expected_author = get_expected_author(some_author)
-        expected_author.name = "updated"
+        expected_author.name = "updated"  # do not put in fixture, as fixture is shared
 
         actual_author = await finalize(
             run_test=lambda Update: Update(Author).one_by_pk(
                 pk_columns={"uuid": some_author.uuid},
                 data={"name": "updated"},
             ),
             columns=all_columns(
                 article_args=get_article_conditional(some_author),
                 comment_args=get_comment_conditional(some_author),
             ),
             session=session,
             session_async=session_async,
         )
 
-        assert_authors_ordered([actual_author], [expected_author])
+        assert_authors_ordered(
+            [actual_author.copy(exclude={"updated_at"})],
+            [expected_author.copy(exclude={"updated_at"})],
+        )
+        assert actual_author.updated_at is not None
+        assert expected_author.updated_at is not None
+        assert actual_author.updated_at > expected_author.updated_at
 
     async def test_returning_default_column(
         self,
         finalize: FinalizeReturning[Update, Author],
         persisted_authors: list[Author],
         session: Client,
         session_async: AsyncClient,
@@ -150,14 +157,15 @@
             session=session,
             session_async=session_async,
         )
 
         assert actual_author.uuid == persisted_authors[0].uuid
 
 
+@mark.asyncio(scope="session")
 class TestMany:
     @mark.parametrize(**FinalizeParams(Update).returning_many())
     @mark.parametrize(**UPDATE_ARGS)
     async def test_updating_an_existing_model(
         self,
         finalize: FinalizeReturning[Update, list[Author]],
         persisted_authors: list[Author],
@@ -279,14 +287,15 @@
             session=session,
             session_async=session_async,
         )
 
         assert actual_affected_rows == expected_affected_rows
 
 
+@mark.asyncio(scope="session")
 class TestManyDistinct:
     @mark.parametrize(**FinalizeParams(Update).returning_many_distinct())
     @mark.parametrize(**UPDATE_DISTINCT_ARGS)
     async def test_updating_an_existing_model(
         self,
         finalize: FinalizeReturning[Update, list[list[Author]]],
         persisted_authors: list[Author],
```

### Comparing `cuckoo-hasura-0.1.6/tests/test_utils.py` & `cuckoo-hasura-0.1.7/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Generator
 
-from pytest import raises, mark
 from geojson_pydantic import Point
+from pytest import mark, raises
 
-from cuckoo.utils import Prop, grouper, to_truncated_str, to_sql_function_args
+from cuckoo.utils import Prop, grouper, to_sql_function_args, to_truncated_str
 
 
 class TestToTruncatedStr:
     def test_string_longer_than_limit_gets_truncated(self):
         test_input = "A" * 2000
         expected = "A" * 1000 + "..."
```

