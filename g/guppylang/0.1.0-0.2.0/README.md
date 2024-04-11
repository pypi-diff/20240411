# Comparing `tmp/guppylang-0.1.0.tar.gz` & `tmp/guppylang-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guppylang-0.1.0.tar", max compression
+gzip compressed data, was "guppylang-0.2.0.tar", max compression
```

## Comparing `guppylang-0.1.0.tar` & `guppylang-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,55 @@
--rw-r--r--   0        0        0     2564 2024-01-19 16:38:34.187786 guppylang-0.1.0/README.md
--rw-r--r--   0        0        0      240 2024-01-19 16:30:37.875775 guppylang-0.1.0/guppylang/__init__.py
--rw-r--r--   0        0        0    10852 2024-01-17 16:04:12.542128 guppylang-0.1.0/guppylang/ast_util.py
--rw-r--r--   0        0        0        0 2024-01-17 16:04:12.542170 guppylang-0.1.0/guppylang/cfg/__init__.py
--rw-r--r--   0        0        0     6805 2024-01-17 16:04:12.542463 guppylang-0.1.0/guppylang/cfg/analysis.py
--rw-r--r--   0        0        0     5600 2024-01-17 16:04:12.542740 guppylang-0.1.0/guppylang/cfg/bb.py
--rw-r--r--   0        0        0    20104 2024-01-18 17:11:50.392427 guppylang-0.1.0/guppylang/cfg/builder.py
--rw-r--r--   0        0        0     2034 2024-01-17 16:04:12.543305 guppylang-0.1.0/guppylang/cfg/cfg.py
--rw-r--r--   0        0        0        0 2024-01-17 16:04:12.543360 guppylang-0.1.0/guppylang/checker/__init__.py
--rw-r--r--   0        0        0     9316 2024-01-18 17:11:50.392740 guppylang-0.1.0/guppylang/checker/cfg_checker.py
--rw-r--r--   0        0        0     6274 2024-01-17 16:04:12.543816 guppylang-0.1.0/guppylang/checker/core.py
--rw-r--r--   0        0        0    38743 2024-01-18 17:30:09.335566 guppylang-0.1.0/guppylang/checker/expr_checker.py
--rw-r--r--   0        0        0     7772 2024-01-17 16:04:12.544271 guppylang-0.1.0/guppylang/checker/func_checker.py
--rw-r--r--   0        0        0     6432 2024-01-17 16:04:12.544525 guppylang-0.1.0/guppylang/checker/stmt_checker.py
--rw-r--r--   0        0        0        0 2024-01-17 16:04:12.544585 guppylang-0.1.0/guppylang/compiler/__init__.py
--rw-r--r--   0        0        0     6743 2024-01-17 16:04:12.544807 guppylang-0.1.0/guppylang/compiler/cfg_compiler.py
--rw-r--r--   0        0        0     3561 2024-01-17 16:04:12.544935 guppylang-0.1.0/guppylang/compiler/core.py
--rw-r--r--   0        0        0    13374 2024-01-18 17:30:09.335844 guppylang-0.1.0/guppylang/compiler/expr_compiler.py
--rw-r--r--   0        0        0     4444 2024-01-17 16:04:12.545408 guppylang-0.1.0/guppylang/compiler/func_compiler.py
--rw-r--r--   0        0        0     3501 2024-01-17 16:04:12.545672 guppylang-0.1.0/guppylang/compiler/stmt_compiler.py
--rw-r--r--   0        0        0     8784 2024-01-17 16:04:12.545965 guppylang-0.1.0/guppylang/custom.py
--rw-r--r--   0        0        0     3051 2024-01-17 16:04:12.546299 guppylang-0.1.0/guppylang/declared.py
--rw-r--r--   0        0        0    10190 2024-01-19 16:12:55.170456 guppylang-0.1.0/guppylang/decorator.py
--rw-r--r--   0        0        0     6245 2024-01-18 17:11:50.393134 guppylang-0.1.0/guppylang/error.py
--rw-r--r--   0        0        0    20768 2024-01-17 16:04:12.546970 guppylang-0.1.0/guppylang/gtypes.py
--rw-r--r--   0        0        0        0 2024-01-17 16:04:12.547029 guppylang-0.1.0/guppylang/hugr/__init__.py
--rw-r--r--   0        0        0    28714 2024-01-19 15:49:57.632826 guppylang-0.1.0/guppylang/hugr/hugr.py
--rw-r--r--   0        0        0    14959 2024-01-17 16:04:12.547796 guppylang-0.1.0/guppylang/hugr/ops.py
--rw-r--r--   0        0        0      567 2024-01-19 15:49:57.633079 guppylang-0.1.0/guppylang/hugr/raw.py
--rw-r--r--   0        0        0     7476 2024-01-17 16:04:12.547993 guppylang-0.1.0/guppylang/hugr/tys.py
--rw-r--r--   0        0        0     1340 2024-01-17 16:04:12.548095 guppylang-0.1.0/guppylang/hugr/val.py
--rw-r--r--   0        0        0     8181 2024-01-17 16:04:12.548273 guppylang-0.1.0/guppylang/hugr/visualise.py
--rw-r--r--   0        0        0    11369 2024-01-19 15:46:16.162365 guppylang-0.1.0/guppylang/module.py
--rw-r--r--   0        0        0     3776 2024-01-17 16:04:12.548668 guppylang-0.1.0/guppylang/nodes.py
--rw-r--r--   0        0        0        0 2024-01-17 16:04:12.548704 guppylang-0.1.0/guppylang/prelude/__init__.py
--rw-r--r--   0        0        0    11151 2024-01-17 18:02:07.622366 guppylang-0.1.0/guppylang/prelude/_internal.py
--rw-r--r--   0        0        0    23305 2024-01-17 16:04:12.549010 guppylang-0.1.0/guppylang/prelude/builtins.py
--rw-r--r--   0        0        0     2622 2024-01-17 18:02:07.622683 guppylang-0.1.0/guppylang/prelude/quantum.py
--rw-r--r--   0        0        0     1098 2024-01-19 16:42:44.000723 guppylang-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 guppylang-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-03-06 14:35:45.141750 guppylang-0.2.0/guppylang/__init__.py
+-rw-r--r--   0        0        0    10848 2024-03-19 17:26:38.074513 guppylang-0.2.0/guppylang/ast_util.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.099571 guppylang-0.2.0/guppylang/cfg/__init__.py
+-rw-r--r--   0        0        0     6805 2024-01-18 13:08:34.099799 guppylang-0.2.0/guppylang/cfg/analysis.py
+-rw-r--r--   0        0        0     5600 2024-01-18 13:08:34.099944 guppylang-0.2.0/guppylang/cfg/bb.py
+-rw-r--r--   0        0        0    20103 2024-03-19 17:26:38.075014 guppylang-0.2.0/guppylang/cfg/builder.py
+-rw-r--r--   0        0        0     2034 2024-01-18 13:08:34.100296 guppylang-0.2.0/guppylang/cfg/cfg.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.100352 guppylang-0.2.0/guppylang/checker/__init__.py
+-rw-r--r--   0        0        0     9281 2024-04-10 12:30:34.670288 guppylang-0.2.0/guppylang/checker/cfg_checker.py
+-rw-r--r--   0        0        0     6958 2024-04-10 12:30:34.670754 guppylang-0.2.0/guppylang/checker/core.py
+-rw-r--r--   0        0        0    40940 2024-04-10 12:30:34.671870 guppylang-0.2.0/guppylang/checker/expr_checker.py
+-rw-r--r--   0        0        0     7887 2024-04-10 12:30:34.672400 guppylang-0.2.0/guppylang/checker/func_checker.py
+-rw-r--r--   0        0        0     6466 2024-03-19 17:26:38.077637 guppylang-0.2.0/guppylang/checker/stmt_checker.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.101552 guppylang-0.2.0/guppylang/compiler/__init__.py
+-rw-r--r--   0        0        0     6881 2024-04-10 12:30:34.672984 guppylang-0.2.0/guppylang/compiler/cfg_compiler.py
+-rw-r--r--   0        0        0     3592 2024-04-10 12:30:34.673508 guppylang-0.2.0/guppylang/compiler/core.py
+-rw-r--r--   0        0        0    13938 2024-04-10 12:34:58.734322 guppylang-0.2.0/guppylang/compiler/expr_compiler.py
+-rw-r--r--   0        0        0     4497 2024-04-10 12:30:34.675115 guppylang-0.2.0/guppylang/compiler/func_compiler.py
+-rw-r--r--   0        0        0     3501 2024-03-19 17:26:38.078950 guppylang-0.2.0/guppylang/compiler/stmt_compiler.py
+-rw-r--r--   0        0        0     9000 2024-04-10 12:30:34.675423 guppylang-0.2.0/guppylang/custom.py
+-rw-r--r--   0        0        0     3066 2024-04-10 12:30:34.675833 guppylang-0.2.0/guppylang/declared.py
+-rw-r--r--   0        0        0     8741 2024-04-10 12:30:34.676264 guppylang-0.2.0/guppylang/decorator.py
+-rw-r--r--   0        0        0     6043 2024-03-19 17:26:38.079877 guppylang-0.2.0/guppylang/error.py
+-rw-r--r--   0        0        0        0 2024-01-30 13:18:23.816770 guppylang-0.2.0/guppylang/graph.hugr
+-rw-r--r--   0        0        0     2903 2024-04-09 09:34:36.229984 guppylang-0.2.0/guppylang/graph.json
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.102977 guppylang-0.2.0/guppylang/hugr/__init__.py
+-rw-r--r--   0        0        0    28695 2024-03-19 17:26:38.080208 guppylang-0.2.0/guppylang/hugr/hugr.py
+-rw-r--r--   0        0        0    14938 2024-03-19 17:26:38.080533 guppylang-0.2.0/guppylang/hugr/ops.py
+-rw-r--r--   0        0        0      567 2024-01-30 09:26:54.831969 guppylang-0.2.0/guppylang/hugr/raw.py
+-rw-r--r--   0        0        0     7476 2024-04-09 09:42:13.717116 guppylang-0.2.0/guppylang/hugr/tys.py
+-rw-r--r--   0        0        0     1340 2024-01-18 13:08:34.103710 guppylang-0.2.0/guppylang/hugr/val.py
+-rw-r--r--   0        0        0     8182 2024-03-19 14:02:30.181552 guppylang-0.2.0/guppylang/hugr/visualise.py
+-rw-r--r--   0        0        0    11390 2024-04-10 12:30:34.676681 guppylang-0.2.0/guppylang/module.py
+-rw-r--r--   0        0        0     3773 2024-04-10 12:30:34.677122 guppylang-0.2.0/guppylang/nodes.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.104139 guppylang-0.2.0/guppylang/prelude/__init__.py
+-rw-r--r--   0        0        0    11676 2024-04-10 12:34:58.734743 guppylang-0.2.0/guppylang/prelude/_internal.py
+-rw-r--r--   0        0        0    22151 2024-04-10 12:30:34.677590 guppylang-0.2.0/guppylang/prelude/builtins.py
+-rw-r--r--   0        0        0     2566 2024-04-11 09:51:54.533323 guppylang-0.2.0/guppylang/prelude/quantum.py
+-rw-r--r--   0        0        0        0 2024-03-04 15:19:40.627545 guppylang-0.2.0/guppylang/py.typed
+-rw-r--r--   0        0        0    10347 2024-04-09 09:34:36.108313 guppylang-0.2.0/guppylang/test
+-rw-r--r--   0        0        0    20574 2024-04-09 09:34:36.224964 guppylang-0.2.0/guppylang/test.svg
+-rw-r--r--   0        0        0        0 2024-03-19 17:26:38.082129 guppylang-0.2.0/guppylang/tys/__init__.py
+-rw-r--r--   0        0        0     2934 2024-03-19 17:26:38.082454 guppylang-0.2.0/guppylang/tys/arg.py
+-rw-r--r--   0        0        0     1835 2024-03-19 17:26:38.082672 guppylang-0.2.0/guppylang/tys/common.py
+-rw-r--r--   0        0        0     1860 2024-03-19 17:26:38.082879 guppylang-0.2.0/guppylang/tys/const.py
+-rw-r--r--   0        0        0     6593 2024-04-10 12:30:34.679407 guppylang-0.2.0/guppylang/tys/definition.py
+-rw-r--r--   0        0        0     5826 2024-03-19 17:26:38.083313 guppylang-0.2.0/guppylang/tys/param.py
+-rw-r--r--   0        0        0     4447 2024-04-10 12:30:34.680034 guppylang-0.2.0/guppylang/tys/parsing.py
+-rw-r--r--   0        0        0     4390 2024-03-19 17:26:38.083753 guppylang-0.2.0/guppylang/tys/printing.py
+-rw-r--r--   0        0        0     2209 2024-03-19 17:26:38.083922 guppylang-0.2.0/guppylang/tys/subst.py
+-rw-r--r--   0        0        0    18580 2024-04-10 12:30:34.680493 guppylang-0.2.0/guppylang/tys/ty.py
+-rw-r--r--   0        0        0     1174 2024-03-19 17:26:38.084390 guppylang-0.2.0/guppylang/tys/var.py
+-rw-r--r--   0        0        0     1173 2024-04-11 09:51:54.533542 guppylang-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      646 2024-03-06 14:35:45.146062 guppylang-0.2.0/quickstart.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 guppylang-0.2.0/PKG-INFO
```

### Comparing `guppylang-0.1.0/guppylang/ast_util.py` & `guppylang-0.2.0/guppylang/ast_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 import textwrap
 from collections.abc import Callable, Mapping, Sequence
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Generic, Optional, TypeVar, cast
 
 if TYPE_CHECKING:
-    from guppylang.gtypes import GuppyType
+    from guppylang.tys.ty import Type
 
 AstNode = (
     ast.AST
     | ast.operator
     | ast.expr
     | ast.arg
     | ast.stmt
@@ -282,32 +282,32 @@
 
 def with_loc(loc: ast.AST, node: A) -> A:
     """Copy source location from one AST node to the other."""
     set_location_from(node, loc)
     return node
 
 
-def with_type(ty: "GuppyType", node: A) -> A:
+def with_type(ty: "Type", node: A) -> A:
     """Annotates an AST node with a type."""
     node.type = ty  # type: ignore[attr-defined]
     return node
 
 
-def get_type_opt(node: AstNode) -> Optional["GuppyType"]:
+def get_type_opt(node: AstNode) -> Optional["Type"]:
     """Tries to retrieve a type annotation from an AST node."""
-    from guppylang.gtypes import GuppyType
+    from guppylang.tys.ty import Type, TypeBase
 
     try:
         ty = node.type  # type: ignore[union-attr]
-        return ty if isinstance(ty, GuppyType) else None
+        return cast(Type, ty) if isinstance(ty, TypeBase) else None
     except AttributeError:
         return None
 
 
-def get_type(node: AstNode) -> "GuppyType":
+def get_type(node: AstNode) -> "Type":
     """Retrieve a type annotation from an AST node.
 
     Fails if the node is not annotated.
     """
     ty = get_type_opt(node)
     assert ty is not None
     return ty
```

### Comparing `guppylang-0.1.0/guppylang/cfg/analysis.py` & `guppylang-0.2.0/guppylang/cfg/analysis.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.1.0/guppylang/cfg/bb.py` & `guppylang-0.2.0/guppylang/cfg/bb.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.1.0/guppylang/cfg/builder.py` & `guppylang-0.2.0/guppylang/cfg/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,25 @@
     template_replace,
     with_loc,
 )
 from guppylang.cfg.bb import BB, BBStatement
 from guppylang.cfg.cfg import CFG
 from guppylang.checker.core import Globals
 from guppylang.error import GuppyError, InternalGuppyError
-from guppylang.gtypes import NoneType
 from guppylang.nodes import (
     DesugaredGenerator,
     DesugaredListComp,
     IterEnd,
     IterHasNext,
     IterNext,
     MakeIter,
     NestedFunctionDef,
     PyExpr,
 )
+from guppylang.tys.ty import NoneType
 
 # In order to build expressions, need an endless stream of unique temporary variables
 # to store intermediate results
 tmp_vars: Iterator[str] = (f"%tmp{i}" for i in itertools.count())
 
 
 def is_tmp_var(x: str) -> bool:
@@ -209,15 +209,15 @@
 
     def visit_FunctionDef(
         self, node: ast.FunctionDef, bb: BB, jumps: Jumps
     ) -> BB | None:
         from guppylang.checker.func_checker import check_signature
 
         func_ty = check_signature(node, self.globals)
-        returns_none = isinstance(func_ty.returns, NoneType)
+        returns_none = isinstance(func_ty.output, NoneType)
         cfg = CFGBuilder().build(node.body, returns_none, self.globals)
 
         new_node = NestedFunctionDef(
             cfg,
             func_ty,
             name=node.name,
             args=node.args,
```

### Comparing `guppylang-0.1.0/guppylang/cfg/cfg.py` & `guppylang-0.2.0/guppylang/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.1.0/guppylang/checker/cfg_checker.py` & `guppylang-0.2.0/guppylang/checker/cfg_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from guppylang.ast_util import line_col
 from guppylang.cfg.bb import BB
 from guppylang.cfg.cfg import CFG, BaseCFG
 from guppylang.checker.core import Context, Globals, Locals, Variable
 from guppylang.checker.expr_checker import ExprSynthesizer, to_bool
 from guppylang.checker.stmt_checker import StmtChecker
 from guppylang.error import GuppyError
-from guppylang.gtypes import GuppyType
+from guppylang.tys.ty import Type
 
 VarRow = Sequence[Variable]
 
 
 @dataclass(frozen=True)
 class Signature:
     """The signature of a basic block.
@@ -40,25 +40,25 @@
 class CheckedBB(BB):
     """Basic block annotated with an input and output type signature."""
 
     sig: Signature = Signature.empty()  # noqa: RUF009
 
 
 class CheckedCFG(BaseCFG[CheckedBB]):
-    input_tys: list[GuppyType]
-    output_ty: GuppyType
+    input_tys: list[Type]
+    output_ty: Type
 
-    def __init__(self, input_tys: list[GuppyType], output_ty: GuppyType) -> None:
+    def __init__(self, input_tys: list[Type], output_ty: Type) -> None:
         super().__init__([])
         self.input_tys = input_tys
         self.output_ty = output_ty
 
 
 def check_cfg(
-    cfg: CFG, inputs: VarRow, return_ty: GuppyType, globals: Globals
+    cfg: CFG, inputs: VarRow, return_ty: Type, globals: Globals
 ) -> CheckedCFG:
     """Type checks a control-flow graph.
 
     Annotates the basic blocks with input and output type signatures and removes
     unreachable blocks.
     """
     # First, we need to run program analysis
@@ -117,15 +117,15 @@
     return checked_cfg
 
 
 def check_bb(
     bb: BB,
     checked_cfg: CheckedCFG,
     inputs: VarRow,
-    return_ty: GuppyType,
+    return_ty: Type,
     globals: Globals,
 ) -> CheckedBB:
     cfg = bb.containing_cfg
 
     # For the entry BB we have to separately check that all used variables are
     # defined. For all other BBs, this will be checked when compiling a predecessor.
     if bb == cfg.entry_bb:
```

### Comparing `guppylang-0.1.0/guppylang/checker/core.py` & `guppylang-0.2.0/guppylang/checker/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,54 +2,66 @@
 import copy
 import itertools
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
 from typing import Any, NamedTuple
 
+from typing_extensions import assert_never
+
 from guppylang.ast_util import AstNode, name_nodes_in_ast
-from guppylang.gtypes import (
-    BoolType,
+from guppylang.tys.definition import (
+    TypeDef,
+    bool_type_def,
+    callable_type_def,
+    linst_type_def,
+    list_type_def,
+    none_type_def,
+    tuple_type_def,
+)
+from guppylang.tys.param import Parameter
+from guppylang.tys.subst import Subst
+from guppylang.tys.ty import (
+    BoundTypeVar,
+    ExistentialTypeVar,
     FunctionType,
-    GuppyType,
-    LinstType,
-    ListType,
     NoneType,
-    Subst,
+    OpaqueType,
     SumType,
     TupleType,
+    Type,
 )
 
 
 @dataclass
 class Variable:
     """Class holding data associated with a variable."""
 
     name: str
-    ty: GuppyType
+    ty: Type
     defined_at: AstNode | None
     used: AstNode | None
 
 
 @dataclass
 class CallableVariable(ABC, Variable):
     """Abstract base class for global variables that can be called."""
 
     ty: FunctionType
 
     @abstractmethod
     def check_call(
-        self, args: list[ast.expr], ty: GuppyType, node: AstNode, ctx: "Context"
+        self, args: list[ast.expr], ty: Type, node: AstNode, ctx: "Context"
     ) -> tuple[ast.expr, Subst]:
         """Checks the return type of a function call against a given type."""
 
     @abstractmethod
     def synthesize_call(
         self, args: list[ast.expr], node: AstNode, ctx: "Context"
-    ) -> tuple[ast.expr, GuppyType]:
+    ) -> tuple[ast.expr, Type]:
         """Synthesizes the return type of a function call."""
 
 
 @dataclass
 class TypeVarDecl:
     """A declared type variable."""
 
@@ -64,56 +76,70 @@
     """Collection of names that are available on module-level.
 
     Separately stores names that are bound to values (i.e. module-level functions or
     constants), to types, or to instance functions belonging to types.
     """
 
     values: dict[str, Variable]
-    types: dict[str, type[GuppyType]]
-    type_vars: dict[str, TypeVarDecl]
+    type_defs: dict[str, TypeDef]
+    param_vars: dict[str, Parameter]
     python_scope: PyScope
 
     @staticmethod
     def default() -> "Globals":
         """Generates a `Globals` instance that is populated with all core types"""
-        tys: dict[str, type[GuppyType]] = {
-            FunctionType.name: FunctionType,
-            TupleType.name: TupleType,
-            SumType.name: SumType,
-            NoneType.name: NoneType,
-            BoolType.name: BoolType,
-            ListType.name: ListType,
-            LinstType.name: LinstType,
+        type_defs = {
+            "Callable": callable_type_def,
+            "tuple": tuple_type_def,
+            "None": none_type_def,
+            "bool": bool_type_def,
+            "list": list_type_def,
+            "linst": linst_type_def,
         }
-        return Globals({}, tys, {}, {})
+        return Globals({}, type_defs, {}, {})
 
-    def get_instance_func(self, ty: GuppyType, name: str) -> CallableVariable | None:
+    def get_instance_func(self, ty: Type, name: str) -> CallableVariable | None:
         """Looks up an instance function with a given name for a type.
 
         Returns `None` if the name doesn't exist or isn't a function.
         """
-        qualname = qualified_name(ty.__class__, name)
+        defn: TypeDef
+        match ty:
+            case BoundTypeVar() | ExistentialTypeVar() | SumType():
+                return None
+            case FunctionType():
+                defn = callable_type_def
+            case OpaqueType() as ty:
+                defn = ty.defn
+            case TupleType():
+                defn = tuple_type_def
+            case NoneType():
+                defn = none_type_def
+            case _:
+                assert_never(ty)
+
+        qualname = qualified_name(defn.name, name)
         if qualname in self.values:
             val = self.values[qualname]
             if isinstance(val, CallableVariable):
                 return val
         return None
 
     def __or__(self, other: "Globals") -> "Globals":
         return Globals(
             self.values | other.values,
-            self.types | other.types,
-            self.type_vars | other.type_vars,
+            self.type_defs | other.type_defs,
+            self.param_vars | other.param_vars,
             self.python_scope | other.python_scope,
         )
 
     def __ior__(self, other: "Globals") -> "Globals":  # noqa: PYI034
         self.values.update(other.values)
-        self.types.update(other.types)
-        self.type_vars.update(other.type_vars)
+        self.type_defs.update(other.type_defs)
+        self.param_vars.update(other.param_vars)
         return self
 
 
 @dataclass
 class Locals:
     """Scoped mapping from names to variables"""
 
@@ -199,11 +225,11 @@
 
     def __contains__(self, key: object) -> bool:
         if isinstance(key, str) and key in self.ctx.locals:
             return True
         return super().__contains__(key)
 
 
-def qualified_name(ty: type[GuppyType] | str, name: str) -> str:
+def qualified_name(ty: TypeDef | str, name: str) -> str:
     """Returns a qualified name for an instance function on a type."""
     ty_name = ty if isinstance(ty, str) else ty.name
     return f"{ty_name}.{name}"
```

### Comparing `guppylang-0.1.0/guppylang/checker/expr_checker.py` & `guppylang-0.2.0/guppylang/checker/expr_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,41 +45,50 @@
 )
 from guppylang.error import (
     GuppyError,
     GuppyTypeError,
     GuppyTypeInferenceError,
     InternalGuppyError,
 )
-from guppylang.gtypes import (
-    BoolType,
-    ExistentialTypeVar,
-    FunctionType,
-    GuppyType,
-    Inst,
-    LinstType,
-    ListType,
-    NoneType,
-    Subst,
-    TupleType,
-    row_to_type,
-    unify,
-)
 from guppylang.nodes import (
     DesugaredGenerator,
     DesugaredListComp,
     GlobalName,
     IterEnd,
     IterHasNext,
     IterNext,
     LocalCall,
     LocalName,
     MakeIter,
     PyExpr,
     TypeApply,
 )
+from guppylang.tys.arg import TypeArg
+from guppylang.tys.definition import (
+    bool_type,
+    get_element_type,
+    is_bool_type,
+    is_linst_type,
+    is_list_type,
+    linst_type,
+    list_type,
+)
+from guppylang.tys.param import TypeParam
+from guppylang.tys.subst import Inst, Subst
+from guppylang.tys.ty import (
+    ExistentialTypeVar,
+    FunctionType,
+    NoneType,
+    OpaqueType,
+    TupleType,
+    Type,
+    TypeBase,
+    row_to_type,
+    unify,
+)
 
 # Mapping from unary AST op to dunder method and display name
 unary_table: dict[type[ast.unaryop], tuple[str, str]] = {
     ast.UAdd:   ("__pos__",    "+"),
     ast.USub:   ("__neg__",    "-"),
     ast.Invert: ("__invert__", "~"),
 }  # fmt: skip
@@ -124,30 +133,30 @@
 
     def __init__(self, ctx: Context) -> None:
         self.ctx = ctx
         self._kind = "expression"
 
     def _fail(
         self,
-        expected: GuppyType,
-        actual: ast.expr | GuppyType,
+        expected: Type,
+        actual: ast.expr | Type,
         loc: AstNode | None = None,
     ) -> NoReturn:
         """Raises a type error indicating that the type doesn't match."""
-        if not isinstance(actual, GuppyType):
+        if not isinstance(actual, TypeBase):
             loc = loc or actual
             _, actual = self._synthesize(actual, allow_free_vars=True)
         if loc is None:
             raise InternalGuppyError("Failure location is required")
         raise GuppyTypeError(
             f"Expected {self._kind} of type `{expected}`, got `{actual}`", loc
         )
 
     def check(
-        self, expr: ast.expr, ty: GuppyType, kind: str = "expression"
+        self, expr: ast.expr, ty: Type, kind: str = "expression"
     ) -> tuple[ast.expr, Subst]:
         """Checks an expression against a type.
 
         The type may have free type variables which will try to be resolved. Returns
         a new desugared expression with type annotations and a substitution with the
         resolved type variables.
         """
@@ -169,49 +178,50 @@
         self._kind = kind or self._kind
         expr, subst = self.visit(expr, ty)
         self._kind = old_kind
         return with_type(ty.substitute(subst), expr), subst
 
     def _synthesize(
         self, node: ast.expr, allow_free_vars: bool
-    ) -> tuple[ast.expr, GuppyType]:
+    ) -> tuple[ast.expr, Type]:
         """Invokes the type synthesiser"""
         return ExprSynthesizer(self.ctx).synthesize(node, allow_free_vars)
 
-    def visit_Tuple(self, node: ast.Tuple, ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def visit_Tuple(self, node: ast.Tuple, ty: Type) -> tuple[ast.expr, Subst]:
         if not isinstance(ty, TupleType) or len(ty.element_types) != len(node.elts):
             return self._fail(ty, node)
         subst: Subst = {}
         for i, el in enumerate(node.elts):
             node.elts[i], s = self.check(el, ty.element_types[i].substitute(subst))
             subst |= s
         return node, subst
 
-    def visit_List(self, node: ast.List, ty: GuppyType) -> tuple[ast.expr, Subst]:
-        if not isinstance(ty, ListType | LinstType):
+    def visit_List(self, node: ast.List, ty: Type) -> tuple[ast.expr, Subst]:
+        if not is_list_type(ty) and not is_linst_type(ty):
             return self._fail(ty, node)
+        el_ty = get_element_type(ty)
         subst: Subst = {}
         for i, el in enumerate(node.elts):
-            node.elts[i], s = self.check(el, ty.element_type.substitute(subst))
+            node.elts[i], s = self.check(el, el_ty.substitute(subst))
             subst |= s
         return node, subst
 
     def visit_DesugaredListComp(
-        self, node: DesugaredListComp, ty: GuppyType
+        self, node: DesugaredListComp, ty: Type
     ) -> tuple[ast.expr, Subst]:
-        if not isinstance(ty, ListType | LinstType):
+        if not is_list_type(ty) and not is_linst_type(ty):
             return self._fail(ty, node)
         node, elt_ty = synthesize_comprehension(node, node.generators, self.ctx)
-        subst = unify(ty.element_type, elt_ty, {})
+        subst = unify(get_element_type(ty), elt_ty, {})
         if subst is None:
-            actual = LinstType(elt_ty) if elt_ty.linear else ListType(elt_ty)
+            actual = linst_type(elt_ty) if elt_ty.linear else list_type(elt_ty)
             return self._fail(ty, actual, node)
         return node, subst
 
-    def visit_Call(self, node: ast.Call, ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def visit_Call(self, node: ast.Call, ty: Type) -> tuple[ast.expr, Subst]:
         if len(node.keywords) > 0:
             raise GuppyError(
                 "Argument passing by keyword is not supported", node.keywords[0]
             )
         node.func, func_ty = self._synthesize(node.func, allow_free_vars=False)
 
         # First handle direct calls of user-defined functions and extension functions
@@ -227,61 +237,76 @@
             node.func = instantiate_poly(node.func, func_ty, inst)
             return with_loc(node, LocalCall(func=node.func, args=args)), return_ty
         elif f := self.ctx.globals.get_instance_func(func_ty, "__call__"):
             return f.check_call(node.args, ty, node, self.ctx)
         else:
             raise GuppyTypeError(f"Expected function type, got `{func_ty}`", node.func)
 
-    def generic_visit(self, node: ast.expr, ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def visit_PyExpr(self, node: PyExpr, ty: Type) -> tuple[ast.expr, Subst]:
+        python_val = eval_py_expr(node, self.ctx)
+        if act := python_value_to_guppy_type(python_val, node, self.ctx.globals):
+            subst = unify(ty, act, {})
+            if subst is None:
+                self._fail(ty, act, node)
+            act = act.substitute(subst)
+            subst = {x: s for x, s in subst.items() if x in ty.unsolved_vars}
+            return with_type(act, with_loc(node, ast.Constant(value=python_val))), subst
+
+        raise GuppyError(
+            f"Python expression of type `{type(python_val)}` is not supported by Guppy",
+            node,
+        )
+
+    def generic_visit(self, node: ast.expr, ty: Type) -> tuple[ast.expr, Subst]:
         # Try to synthesize and then check if we can unify it with the given type
         node, synth = self._synthesize(node, allow_free_vars=False)
         subst, inst = check_type_against(synth, ty, node, self._kind)
 
         # Apply instantiation of quantified type variables
         if inst:
-            node = with_loc(node, TypeApply(value=node, tys=inst))
+            node = with_loc(node, TypeApply(value=node, inst=inst))
 
         return node, subst
 
 
-class ExprSynthesizer(AstVisitor[tuple[ast.expr, GuppyType]]):
+class ExprSynthesizer(AstVisitor[tuple[ast.expr, Type]]):
     ctx: Context
 
     def __init__(self, ctx: Context) -> None:
         self.ctx = ctx
 
     def synthesize(
         self, node: ast.expr, allow_free_vars: bool = False
-    ) -> tuple[ast.expr, GuppyType]:
+    ) -> tuple[ast.expr, Type]:
         """Tries to synthesise a type for the given expression.
 
         Also returns a new desugared expression with type annotations.
         """
         if ty := get_type_opt(node):
             return node, ty
         node, ty = self.visit(node)
         if ty.unsolved_vars and not allow_free_vars:
             raise GuppyTypeError(
                 f"Cannot infer type variable in expression of type `{ty}`", node
             )
         return with_type(ty, node), ty
 
     def _check(
-        self, expr: ast.expr, ty: GuppyType, kind: str = "expression"
+        self, expr: ast.expr, ty: Type, kind: str = "expression"
     ) -> tuple[ast.expr, Subst]:
         """Checks an expression against a given type"""
         return ExprChecker(self.ctx).check(expr, ty, kind)
 
-    def visit_Constant(self, node: ast.Constant) -> tuple[ast.expr, GuppyType]:
+    def visit_Constant(self, node: ast.Constant) -> tuple[ast.expr, Type]:
         ty = python_value_to_guppy_type(node.value, node, self.ctx.globals)
         if ty is None:
             raise GuppyError("Unsupported constant", node)
         return node, ty
 
-    def visit_Name(self, node: ast.Name) -> tuple[ast.Name, GuppyType]:
+    def visit_Name(self, node: ast.Name) -> tuple[ast.Name, Type]:
         x = node.id
         if x in self.ctx.locals:
             var = self.ctx.locals[x]
             if var.ty.linear and var.used is not None:
                 raise GuppyError(
                     f"Variable `{x}` with linear type `{var.ty}` was "
                     "already used (at {0})",
@@ -295,36 +320,34 @@
             value = self.ctx.globals.values[x]
             return with_loc(node, GlobalName(id=x, value=value)), value.ty
         raise InternalGuppyError(
             f"Variable `{x}` is not defined in `TypeSynthesiser`. This should have "
             f"been caught by program analysis!"
         )
 
-    def visit_Tuple(self, node: ast.Tuple) -> tuple[ast.expr, GuppyType]:
+    def visit_Tuple(self, node: ast.Tuple) -> tuple[ast.expr, Type]:
         elems = [self.synthesize(elem) for elem in node.elts]
         node.elts = [n for n, _ in elems]
         return node, TupleType([ty for _, ty in elems])
 
-    def visit_List(self, node: ast.List) -> tuple[ast.expr, GuppyType]:
+    def visit_List(self, node: ast.List) -> tuple[ast.expr, Type]:
         if len(node.elts) == 0:
             raise GuppyTypeInferenceError(
                 "Cannot infer type variable in expression of type `list[?T]`", node
             )
         node.elts[0], el_ty = self.synthesize(node.elts[0])
         node.elts[1:] = [self._check(el, el_ty)[0] for el in node.elts[1:]]
-        return node, LinstType(el_ty) if el_ty.linear else ListType(el_ty)
+        return node, linst_type(el_ty) if el_ty.linear else list_type(el_ty)
 
-    def visit_DesugaredListComp(
-        self, node: DesugaredListComp
-    ) -> tuple[ast.expr, GuppyType]:
+    def visit_DesugaredListComp(self, node: DesugaredListComp) -> tuple[ast.expr, Type]:
         node, elt_ty = synthesize_comprehension(node, node.generators, self.ctx)
-        result_ty = LinstType(elt_ty) if elt_ty.linear else ListType(elt_ty)
+        result_ty = linst_type(elt_ty) if elt_ty.linear else list_type(elt_ty)
         return node, result_ty
 
-    def visit_UnaryOp(self, node: ast.UnaryOp) -> tuple[ast.expr, GuppyType]:
+    def visit_UnaryOp(self, node: ast.UnaryOp) -> tuple[ast.expr, Type]:
         # We need to synthesise the argument type, so we can look up dunder methods
         node.operand, op_ty = self.synthesize(node.operand)
 
         # Special case for the `not` operation since it is not implemented via a dunder
         # method or control-flow
         if isinstance(node.op, ast.Not):
             node.operand, bool_ty = to_bool(node.operand, op_ty, self.ctx)
@@ -339,15 +362,15 @@
                 f" `{op_ty}`",
                 node.operand,
             )
         return func.synthesize_call([node.operand], node, self.ctx)
 
     def _synthesize_binary(
         self, left_expr: ast.expr, right_expr: ast.expr, op: AstOp, node: ast.expr
-    ) -> tuple[ast.expr, GuppyType]:
+    ) -> tuple[ast.expr, Type]:
         """Helper method to compile binary operators by calling out to dunder methods.
 
         For example, first try calling `__add__` on the left operand. If that fails, try
         `__radd__` on the right operand.
         """
         if op.__class__ not in binary_table:
             raise GuppyError("This binary operation is not supported by Guppy.", op)
@@ -373,15 +396,15 @@
         self,
         node: ast.expr,
         args: list[ast.expr],
         func_name: str,
         err: str,
         exp_sig: FunctionType | None = None,
         give_reason: bool = False,
-    ) -> tuple[ast.expr, GuppyType]:
+    ) -> tuple[ast.expr, Type]:
         """Helper method for expressions that are implemented via instance methods.
 
         Raises a `GuppyTypeError` if the given instance method is not defined. The error
         message can be customised by passing an `err` string and an optional error
         reason can be printed.
 
         Optionally, the signature of the instance function can also be checked against a
@@ -393,43 +416,43 @@
             reason = f" since it does not implement the `{func_name}` method"
             raise GuppyTypeError(
                 f"Expression of type `{ty}` is {err}{reason if give_reason else ''}",
                 node,
             )
         if exp_sig and unify(exp_sig, func.ty.unquantified()[0], {}) is None:
             raise GuppyError(
-                f"Method `{ty.name}.{func_name}` has signature `{func.ty}`, but "
+                f"Method `{ty}.{func_name}` has signature `{func.ty}`, but "
                 f"expected `{exp_sig}`",
                 node,
             )
         return func.synthesize_call([node, *args], node, self.ctx)
 
-    def visit_BinOp(self, node: ast.BinOp) -> tuple[ast.expr, GuppyType]:
+    def visit_BinOp(self, node: ast.BinOp) -> tuple[ast.expr, Type]:
         return self._synthesize_binary(node.left, node.right, node.op, node)
 
-    def visit_Compare(self, node: ast.Compare) -> tuple[ast.expr, GuppyType]:
+    def visit_Compare(self, node: ast.Compare) -> tuple[ast.expr, Type]:
         if len(node.comparators) != 1 or len(node.ops) != 1:
             raise InternalGuppyError(
                 "BB contains chained comparison. Should have been removed during CFG "
                 "construction."
             )
         left_expr, [op], [right_expr] = node.left, node.ops, node.comparators
         return self._synthesize_binary(left_expr, right_expr, op, node)
 
-    def visit_Subscript(self, node: ast.Subscript) -> tuple[ast.expr, GuppyType]:
+    def visit_Subscript(self, node: ast.Subscript) -> tuple[ast.expr, Type]:
         node.value, ty = self.synthesize(node.value)
         exp_sig = FunctionType(
-            [ty, ExistentialTypeVar.new("Key", False)],
-            ExistentialTypeVar.new("Val", False),
+            [ty, ExistentialTypeVar.fresh("Key", False)],
+            ExistentialTypeVar.fresh("Val", False),
         )
         return self._synthesize_instance_func(
             node.value, [node.slice], "__getitem__", "not subscriptable", exp_sig
         )
 
-    def visit_Call(self, node: ast.Call) -> tuple[ast.expr, GuppyType]:
+    def visit_Call(self, node: ast.Call) -> tuple[ast.expr, Type]:
         if len(node.keywords) > 0:
             raise GuppyError("Keyword arguments are not supported", node.keywords[0])
         node.func, ty = self.synthesize(node.func)
 
         # First handle direct calls of user-defined functions and extension functions
         if isinstance(node.func, GlobalName) and isinstance(
             node.func.value, CallableVariable
@@ -442,17 +465,17 @@
             node.func = instantiate_poly(node.func, ty, inst)
             return with_loc(node, LocalCall(func=node.func, args=args)), return_ty
         elif f := self.ctx.globals.get_instance_func(ty, "__call__"):
             return f.synthesize_call(node.args, node, self.ctx)
         else:
             raise GuppyTypeError(f"Expected function type, got `{ty}`", node.func)
 
-    def visit_MakeIter(self, node: MakeIter) -> tuple[ast.expr, GuppyType]:
+    def visit_MakeIter(self, node: MakeIter) -> tuple[ast.expr, Type]:
         node.value, ty = self.synthesize(node.value)
-        exp_sig = FunctionType([ty], ExistentialTypeVar.new("Iter", False))
+        exp_sig = FunctionType([ty], ExistentialTypeVar.fresh("Iter", False))
         expr, ty = self._synthesize_instance_func(
             node.value, [], "__iter__", "not iterable", exp_sig
         )
 
         # If the iterator was created by a `for` loop, we can add some extra checks to
         # produce nicer errors for linearity violations. Namely, `break` and `return`
         # are not allowed when looping over a linear iterator (`continue` is allowed)
@@ -464,136 +487,109 @@
                 raise GuppyTypeError(
                     f"Loop over iterator with linear type `{ty}` cannot be terminated "
                     f"prematurely",
                     breaks[0],
                 )
         return expr, ty
 
-    def visit_IterHasNext(self, node: IterHasNext) -> tuple[ast.expr, GuppyType]:
+    def visit_IterHasNext(self, node: IterHasNext) -> tuple[ast.expr, Type]:
         node.value, ty = self.synthesize(node.value)
-        exp_sig = FunctionType([ty], TupleType([BoolType(), ty]))
+        exp_sig = FunctionType([ty], TupleType([bool_type(), ty]))
         return self._synthesize_instance_func(
             node.value, [], "__hasnext__", "not an iterator", exp_sig, True
         )
 
-    def visit_IterNext(self, node: IterNext) -> tuple[ast.expr, GuppyType]:
+    def visit_IterNext(self, node: IterNext) -> tuple[ast.expr, Type]:
         node.value, ty = self.synthesize(node.value)
         exp_sig = FunctionType(
-            [ty], TupleType([ExistentialTypeVar.new("T", False), ty])
+            [ty], TupleType([ExistentialTypeVar.fresh("T", False), ty])
         )
         return self._synthesize_instance_func(
             node.value, [], "__next__", "not an iterator", exp_sig, True
         )
 
-    def visit_IterEnd(self, node: IterEnd) -> tuple[ast.expr, GuppyType]:
+    def visit_IterEnd(self, node: IterEnd) -> tuple[ast.expr, Type]:
         node.value, ty = self.synthesize(node.value)
         exp_sig = FunctionType([ty], NoneType())
         return self._synthesize_instance_func(
             node.value, [], "__end__", "not an iterator", exp_sig, True
         )
 
-    def visit_ListComp(self, node: ast.ListComp) -> tuple[ast.expr, GuppyType]:
+    def visit_ListComp(self, node: ast.ListComp) -> tuple[ast.expr, Type]:
         raise InternalGuppyError(
             "BB contains `ListComp`. Should have been removed during CFG"
             f"construction: `{ast.unparse(node)}`"
         )
 
-    def visit_PyExpr(self, node: PyExpr) -> tuple[ast.expr, GuppyType]:
-        # The method we used for obtaining the Python variables in scope only works in
-        # CPython (see `get_py_scope()`).
-        if sys.implementation.name != "cpython":
-            raise GuppyError(
-                "Compile-time `py(...)` expressions are only supported in CPython", node
-            )
-
-        try:
-            python_val = eval(  # noqa: S307, PGH001
-                ast.unparse(node.value),
-                None,
-                DummyEvalDict(self.ctx, node.value),
-            )
-        except DummyEvalDict.GuppyVarUsedError as e:
-            raise GuppyError(
-                f"Guppy variable `{e.var}` cannot be accessed in a compile-time "
-                "`py(...)` expression",
-                e.node or node,
-            ) from None
-        except Exception as e:  # noqa: BLE001
-            # Remove the top frame pointing to the `eval` call from the stack trace
-            tb = e.__traceback__.tb_next if e.__traceback__ else None
-            raise GuppyError(
-                "Error occurred while evaluating Python expression:\n\n"
-                + "".join(traceback.format_exception(type(e), e, tb)),
-                node,
-            ) from e
-
+    def visit_PyExpr(self, node: PyExpr) -> tuple[ast.expr, Type]:
+        python_val = eval_py_expr(node, self.ctx)
         if ty := python_value_to_guppy_type(python_val, node, self.ctx.globals):
             return with_loc(node, ast.Constant(value=python_val)), ty
 
         raise GuppyError(
             f"Python expression of type `{type(python_val)}` is not supported by Guppy",
             node,
         )
 
-    def visit_NamedExpr(self, node: ast.NamedExpr) -> tuple[ast.expr, GuppyType]:
+    def visit_NamedExpr(self, node: ast.NamedExpr) -> tuple[ast.expr, Type]:
         raise InternalGuppyError(
             "BB contains `NamedExpr`. Should have been removed during CFG"
             f"construction: `{ast.unparse(node)}`"
         )
 
-    def visit_BoolOp(self, node: ast.BoolOp) -> tuple[ast.expr, GuppyType]:
+    def visit_BoolOp(self, node: ast.BoolOp) -> tuple[ast.expr, Type]:
         raise InternalGuppyError(
             "BB contains `BoolOp`. Should have been removed during CFG construction: "
             f"`{ast.unparse(node)}`"
         )
 
-    def visit_IfExp(self, node: ast.IfExp) -> tuple[ast.expr, GuppyType]:
+    def visit_IfExp(self, node: ast.IfExp) -> tuple[ast.expr, Type]:
         raise InternalGuppyError(
             "BB contains `IfExp`. Should have been removed during CFG construction: "
             f"`{ast.unparse(node)}`"
         )
 
 
 def check_type_against(
-    act: GuppyType, exp: GuppyType, node: AstNode, kind: str = "expression"
+    act: Type, exp: Type, node: AstNode, kind: str = "expression"
 ) -> tuple[Subst, Inst]:
     """Checks a type against another type.
 
     Returns a substitution for the free variables the expected type and an instantiation
-    for the quantified variables in the actual type. Note that the expected type may not
-    be quantified and the actual type may not contain free unification variables.
+    for the parameters in the actual type. Note that the expected type may not be
+    parametrised and the actual type may not contain free unification variables.
     """
-    assert not isinstance(exp, FunctionType) or not exp.quantified
+    assert not isinstance(exp, FunctionType) or not exp.parametrized
     assert not act.unsolved_vars
 
-    # The actual type may be quantified. In that case, we have to find an instantiation
-    # to avoid higher-rank types.
+    # The actual type may be parametrised. In that case, we have to find an
+    # instantiation to avoid higher-rank types.
     subst: Subst | None
-    if isinstance(act, FunctionType) and act.quantified:
+    if isinstance(act, FunctionType) and act.parametrized:
         unquantified, free_vars = act.unquantified()
         subst = unify(exp, unquantified, {})
         if subst is None:
             raise GuppyTypeError(f"Expected {kind} of type `{exp}`, got `{act}`", node)
-        # Check that we have found a valid instantiation for all quantified vars
+        # Check that we have found a valid instantiation for all params
         for i, v in enumerate(free_vars):
             if v not in subst:
                 raise GuppyTypeInferenceError(
                     f"Expected {kind} of type `{exp}`, got `{act}`. Couldn't infer an "
-                    f"instantiation for type variable `{act.quantified[i]}` (higher-"
-                    "rank polymorphic types are not supported)",
+                    f"instantiation for parameter `{act.params[i].name}` (higher-rank "
+                    "polymorphic types are not supported)",
                     node,
                 )
             if subst[v].unsolved_vars:
                 raise GuppyTypeError(
                     f"Expected {kind} of type `{exp}`, got `{act}`. Can't instantiate "
-                    f"type variable `{act.quantified[i]}` with type `{subst[v]}` "
-                    "containing free variables",
+                    f"parameter `{act.params[i]}` with type `{subst[v]}` containing "
+                    "free variables",
                     node,
                 )
-        inst = [subst[v] for v in free_vars]
+        inst = [TypeArg(subst[v]) for v in free_vars]
         subst = {v: t for v, t in subst.items() if v in exp.unsolved_vars}
 
         # Finally, check that the instantiation respects the linearity requirements
         check_inst(act, inst, node)
 
         return subst, inst
 
@@ -616,90 +612,90 @@
             raise GuppyTypeError("Unexpected argument", node.args[exp])
         raise GuppyTypeError(
             f"Too many arguments passed (expected {exp}, got {act})", node
         )
 
 
 def type_check_args(
-    args: list[ast.expr],
+    inputs: list[ast.expr],
     func_ty: FunctionType,
     subst: Subst,
     ctx: Context,
     node: AstNode,
 ) -> tuple[list[ast.expr], Subst]:
     """Checks the arguments of a function call and infers free type variables.
 
-    We expect that quantified variables have been replaced with free unification
-    variables. Checks that all unification variables can be inferred.
+    We expect that parameters have been replaced with free unification variables.
+    Checks that all unification variables can be inferred.
     """
-    assert not func_ty.quantified
-    check_num_args(len(func_ty.args), len(args), node)
+    assert not func_ty.parametrized
+    check_num_args(len(func_ty.inputs), len(inputs), node)
 
     new_args: list[ast.expr] = []
-    for arg, ty in zip(args, func_ty.args):
-        a, s = ExprChecker(ctx).check(arg, ty.substitute(subst), "argument")
+    for inp, ty in zip(inputs, func_ty.inputs):
+        a, s = ExprChecker(ctx).check(inp, ty.substitute(subst), "argument")
         new_args.append(a)
         subst |= s
 
     # If the argument check succeeded, this means that we must have found instantiations
-    # for all unification variables occurring in the argument types
-    assert all(set.issubset(arg.unsolved_vars, subst.keys()) for arg in func_ty.args)
+    # for all unification variables occurring in the input types
+    assert all(set.issubset(inp.unsolved_vars, subst.keys()) for inp in func_ty.inputs)
 
     # We also have to check that we found instantiations for all vars in the return type
-    if not set.issubset(func_ty.returns.unsolved_vars, subst.keys()):
+    if not set.issubset(func_ty.output.unsolved_vars, subst.keys()):
         raise GuppyTypeInferenceError(
             f"Cannot infer type variable in expression of type "
-            f"`{func_ty.returns.substitute(subst)}`",
+            f"`{func_ty.output.substitute(subst)}`",
             node,
         )
 
     return new_args, subst
 
 
 def synthesize_call(
     func_ty: FunctionType, args: list[ast.expr], node: AstNode, ctx: Context
-) -> tuple[list[ast.expr], GuppyType, Inst]:
+) -> tuple[list[ast.expr], Type, Inst]:
     """Synthesizes the return type of a function call.
 
     Returns an annotated argument list, the synthesized return type, and an
     instantiation for the quantifiers in the function type.
     """
     assert not func_ty.unsolved_vars
-    check_num_args(len(func_ty.args), len(args), node)
+    check_num_args(len(func_ty.inputs), len(args), node)
 
     # Replace quantified variables with free unification variables and try to infer an
     # instantiation by checking the arguments
     unquantified, free_vars = func_ty.unquantified()
     args, subst = type_check_args(args, unquantified, {}, ctx, node)
 
     # Success implies that the substitution is closed
     assert all(not t.unsolved_vars for t in subst.values())
-    inst = [subst[v] for v in free_vars]
+    inst = [TypeArg(subst[v]) for v in free_vars]
 
     # Finally, check that the instantiation respects the linearity requirements
     check_inst(func_ty, inst, node)
 
-    return args, unquantified.returns.substitute(subst), inst
+    return args, unquantified.output.substitute(subst), inst
 
 
 def check_call(
     func_ty: FunctionType,
-    args: list[ast.expr],
-    ty: GuppyType,
+    inputs: list[ast.expr],
+    ty: Type,
     node: AstNode,
     ctx: Context,
     kind: str = "expression",
 ) -> tuple[list[ast.expr], Subst, Inst]:
     """Checks the return type of a function call against a given type.
 
     Returns an annotated argument list, a substitution for the free variables in the
     expected type, and an instantiation for the quantifiers in the function type.
     """
     assert not func_ty.unsolved_vars
-    check_num_args(len(func_ty.args), len(args), node)
+    check_num_args(len(func_ty.inputs), len(inputs), node)
 
     # When checking, we can use the information from the expected return type to infer
     # some type arguments. However, this pushes errors inwards. For example, given a
     # function `foo: forall T. T -> T`, the following type mismatch would be reported:
     #
     #       x: int = foo(None)
     #                    ^^^^  Expected argument of type `int`, got `None`
@@ -713,110 +709,116 @@
     # information from the expected type, we should do that to improve the error.
 
     # TODO: The approach below can result in exponential runtime in the worst case.
     #  However the bad case, e.g. `x: int = foo(foo(...foo(?)...))`, shouldn't be common
     #  in practice. Can we do better than that?
 
     # First, try to synthesize
-    res: tuple[GuppyType, Inst] | None = None
+    res: tuple[Type, Inst] | None = None
     try:
-        args, synth, inst = synthesize_call(func_ty, args, node, ctx)
+        inputs, synth, inst = synthesize_call(func_ty, inputs, node, ctx)
         res = synth, inst
     except GuppyTypeInferenceError:
         pass
     if res is not None:
         synth, inst = res
         subst = unify(ty, synth, {})
         if subst is None:
             raise GuppyTypeError(f"Expected {kind} of type `{ty}`, got `{synth}`", node)
-        return args, subst, inst
+        return inputs, subst, inst
 
     # If synthesis fails, we try again, this time also using information from the
     # expected return type
     unquantified, free_vars = func_ty.unquantified()
-    subst = unify(ty, unquantified.returns, {})
+    subst = unify(ty, unquantified.output, {})
     if subst is None:
         raise GuppyTypeError(
-            f"Expected {kind} of type `{ty}`, got `{unquantified.returns}`", node
+            f"Expected {kind} of type `{ty}`, got `{unquantified.output}`", node
         )
 
     # Try to infer more by checking against the arguments
-    args, subst = type_check_args(args, unquantified, subst, ctx, node)
+    inputs, subst = type_check_args(inputs, unquantified, subst, ctx, node)
 
     # Also make sure we found an instantiation for all free vars in the type we're
     # checking against
     if not set.issubset(ty.unsolved_vars, subst.keys()):
         raise GuppyTypeInferenceError(
             f"Expected expression of type `{ty}`, got "
-            f"`{func_ty.returns.substitute(subst)}`. Couldn't infer type variables",
+            f"`{func_ty.output.substitute(subst)}`. Couldn't infer type variables",
             node,
         )
 
     # Success implies that the substitution is closed
     assert all(not t.unsolved_vars for t in subst.values())
-    inst = [subst[v] for v in free_vars]
+    inst = [TypeArg(subst[v]) for v in free_vars]
     subst = {v: t for v, t in subst.items() if v in ty.unsolved_vars}
 
     # Finally, check that the instantiation respects the linearity requirements
     check_inst(func_ty, inst, node)
 
-    return args, subst, inst
+    return inputs, subst, inst
 
 
 def check_inst(func_ty: FunctionType, inst: Inst, node: AstNode) -> None:
     """Checks if an instantiation is valid.
 
     Makes sure that the linearity requirements are satisfied.
     """
-    for var, ty in zip(func_ty.quantified, inst):
-        if not var.linear and ty.linear:
+    for param, arg in zip(func_ty.params, inst, strict=True):
+        # Give a more informative error message for linearity issues
+        if (
+            isinstance(param, TypeParam)
+            and isinstance(arg, TypeArg)
+            and arg.ty.linear
+            and not param.can_be_linear
+        ):
             raise GuppyTypeError(
-                f"Cannot instantiate non-linear type variable `{var}` in type "
-                f"`{func_ty}` with linear type `{ty}`",
+                f"Cannot instantiate non-linear type variable `{param.name}` in type "
+                f"`{func_ty}` with linear type `{arg.ty}`",
                 node,
             )
+        # For everything else, we fall back to the default checking implementation
+        param.check_arg(arg, node)
 
 
 def instantiate_poly(node: ast.expr, ty: FunctionType, inst: Inst) -> ast.expr:
     """Instantiates quantified type arguments in a function."""
-    assert len(ty.quantified) == len(inst)
+    assert len(ty.params) == len(inst)
     if len(inst) > 0:
-        node = with_loc(node, TypeApply(value=with_type(ty, node), tys=inst))
+        node = with_loc(node, TypeApply(value=with_type(ty, node), inst=inst))
         return with_type(ty.instantiate(inst), node)
     return node
 
 
-def to_bool(
-    node: ast.expr, node_ty: GuppyType, ctx: Context
-) -> tuple[ast.expr, GuppyType]:
+def to_bool(node: ast.expr, node_ty: Type, ctx: Context) -> tuple[ast.expr, Type]:
     """Tries to turn a node into a bool"""
-    if isinstance(node_ty, BoolType):
+    if is_bool_type(node_ty):
         return node, node_ty
 
     func = ctx.globals.get_instance_func(node_ty, "__bool__")
     if func is None:
         raise GuppyTypeError(
             f"Expression of type `{node_ty}` cannot be interpreted as a `bool`",
             node,
         )
 
     # We could check the return type against bool, but we can give a better error
     # message if we synthesise and compare to bool by hand
     call, return_ty = func.synthesize_call([node], node, ctx)
-    if not isinstance(return_ty, BoolType):
+    if not is_bool_type(return_ty):
         raise GuppyTypeError(
             f"`__bool__` on type `{node_ty}` returns `{return_ty}` instead of `bool`",
             node,
         )
     return call, return_ty
 
 
 def synthesize_comprehension(
     node: DesugaredListComp, gens: list[DesugaredGenerator], ctx: Context
-) -> tuple[DesugaredListComp, GuppyType]:
+) -> tuple[DesugaredListComp, Type]:
     """Helper function to synthesise the element type of a list comprehension."""
     from guppylang.checker.stmt_checker import StmtChecker
 
     def check_linear_use_from_outer_scope(expr: ast.expr, locals: Locals) -> None:
         """Checks if an expression uses a linear variable from an outer scope.
 
         Since the expression is executed multiple times in the inner scope, this would
@@ -895,50 +897,110 @@
     # The iter finalizer is again checked in the outer context
     ctx.locals[gen.iter.id].used = None
     gen.iterend, iterend_ty = ExprSynthesizer(ctx).synthesize(gen.iterend)
     gen.iterend = with_type(iterend_ty, gen.iterend)
     return node, elt_ty
 
 
-def python_value_to_guppy_type(
-    v: Any, node: ast.expr, globals: Globals
-) -> GuppyType | None:
+def eval_py_expr(node: PyExpr, ctx: Context) -> Any:
+    """Evaluates a `py(...)` expression."""
+    # The method we used for obtaining the Python variables in scope only works in
+    # CPython (see `get_py_scope()`).
+    if sys.implementation.name != "cpython":
+        raise GuppyError(
+            "Compile-time `py(...)` expressions are only supported in CPython", node
+        )
+
+    try:
+        python_val = eval(  # noqa: S307, PGH001
+            ast.unparse(node.value),
+            None,
+            DummyEvalDict(ctx, node.value),
+        )
+    except DummyEvalDict.GuppyVarUsedError as e:
+        raise GuppyError(
+            f"Guppy variable `{e.var}` cannot be accessed in a compile-time "
+            "`py(...)` expression",
+            e.node or node,
+        ) from None
+    except Exception as e:  # noqa: BLE001
+        # Remove the top frame pointing to the `eval` call from the stack trace
+        tb = e.__traceback__.tb_next if e.__traceback__ else None
+        raise GuppyError(
+            "Error occurred while evaluating Python expression:\n\n"
+            + "".join(traceback.format_exception(type(e), e, tb)),
+            node,
+        ) from e
+    return python_val
+
+
+def python_value_to_guppy_type(v: Any, node: ast.expr, globals: Globals) -> Type | None:
     """Turns a primitive Python value into a Guppy type.
 
     Returns `None` if the Python value cannot be represented in Guppy.
     """
     match v:
         case bool():
-            return globals.types["bool"].build(node=node)
+            return globals.type_defs["bool"].check_instantiate([])
         case int():
-            return globals.types["int"].build(node=node)
+            return globals.type_defs["int"].check_instantiate([])
         case float():
-            return globals.types["float"].build(node=node)
+            return globals.type_defs["float"].check_instantiate([])
         case tuple(elts):
             tys = [python_value_to_guppy_type(elt, node, globals) for elt in elts]
             if any(ty is None for ty in tys):
                 return None
-            return TupleType(cast(list[GuppyType], tys))
+            return TupleType(cast(list[Type], tys))
+        case list():
+            return _python_list_to_guppy_type(v, node, globals)
         case _:
             # Pytket conversion is an optional feature
             try:
                 import pytket
 
                 if isinstance(v, pytket.circuit.Circuit):
                     # We also need tket2 installed
                     try:
                         import tket2  # type: ignore[import-untyped, import-not-found, unused-ignore]  # noqa: F401
 
-                        qubit = globals.types["Qubit"].build()
+                        qubit = globals.type_defs["qubit"].check_instantiate([])
                         return FunctionType(
                             [qubit] * v.n_qubits,
-                            row_to_type([qubit] * v.n_qubits + [BoolType()] * v.n_bits),
+                            row_to_type(
+                                [qubit] * v.n_qubits + [bool_type()] * v.n_bits
+                            ),
                         )
                     except ImportError:
                         raise GuppyError(
                             "Pytket compatibility requires `tket2` to be installed. "
                             "See https://github.com/CQCL/tket2/tree/main/tket2-py",
                             node,
                         ) from None
             except ImportError:
                 pass
             return None
+
+
+def _python_list_to_guppy_type(
+    vs: list[Any], node: ast.expr, globals: Globals
+) -> OpaqueType | None:
+    """Turns a Python list into a Guppy type.
+
+    Returns `None` if the list contains different types or types that are not
+    representable in Guppy.
+    """
+    if len(vs) == 0:
+        return list_type(ExistentialTypeVar.fresh("T", False))
+
+    # All the list elements must have a unifiable types
+    v, *rest = vs
+    el_ty = python_value_to_guppy_type(v, node, globals)
+    if el_ty is None:
+        return None
+    for v in rest:
+        ty = python_value_to_guppy_type(v, node, globals)
+        if ty is None:
+            return None
+        if (subst := unify(ty, el_ty, {})) is None:
+            raise GuppyError("Python list contains elements with different types", node)
+        el_ty = el_ty.substitute(subst)
+    return list_type(el_ty)
```

### Comparing `guppylang-0.1.0/guppylang/checker/func_checker.py` & `guppylang-0.2.0/guppylang/checker/func_checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,61 +3,60 @@
 For top-level functions, we take the `DefinedFunction` containing the `ast.FunctionDef`
 node straight from the Python AST. We build a CFG, check it, and return a
 `CheckedFunction` containing a `CheckedCFG` with type annotations.
 """
 
 import ast
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 from guppylang.ast_util import AstNode, return_nodes_in_ast, with_loc
 from guppylang.cfg.bb import BB
 from guppylang.cfg.builder import CFGBuilder
 from guppylang.checker.cfg_checker import CheckedCFG, check_cfg
 from guppylang.checker.core import CallableVariable, Context, Globals, Variable
 from guppylang.checker.expr_checker import check_call, synthesize_call
 from guppylang.error import GuppyError
-from guppylang.gtypes import (
-    BoundTypeVar,
-    FunctionType,
-    GuppyType,
-    NoneType,
-    Subst,
-    type_from_ast,
-)
 from guppylang.nodes import CheckedNestedFunctionDef, GlobalCall, NestedFunctionDef
+from guppylang.tys.parsing import type_from_ast
+from guppylang.tys.subst import Subst
+from guppylang.tys.ty import FunctionType, NoneType, Type
+
+if TYPE_CHECKING:
+    from guppylang.tys.param import Parameter
 
 
 @dataclass
 class DefinedFunction(CallableVariable):
     """A user-defined function"""
 
     ty: FunctionType
     defined_at: ast.FunctionDef
 
     @staticmethod
     def from_ast(
         func_def: ast.FunctionDef, name: str, globals: Globals
     ) -> "DefinedFunction":
         ty = check_signature(func_def, globals)
-        if ty.quantified:
+        if ty.parametrized:
             raise GuppyError(
                 "Generic function definitions are not supported yet", func_def
             )
         return DefinedFunction(name, ty, func_def, None)
 
     def check_call(
-        self, args: list[ast.expr], ty: GuppyType, node: AstNode, ctx: Context
+        self, args: list[ast.expr], ty: Type, node: AstNode, ctx: Context
     ) -> tuple[ast.expr, Subst]:
         # Use default implementation from the expression checker
         args, subst, inst = check_call(self.ty, args, ty, node, ctx)
         return with_loc(node, GlobalCall(func=self, args=args, type_args=inst)), subst
 
     def synthesize_call(
         self, args: list[ast.expr], node: AstNode, ctx: Context
-    ) -> tuple[GlobalCall, GuppyType]:
+    ) -> tuple[GlobalCall, Type]:
         # Use default implementation from the expression checker
         args, ty, inst = synthesize_call(self.ty, args, node, ctx)
         return with_loc(node, GlobalCall(func=self, args=args, type_args=inst)), ty
 
 
 @dataclass
 class CheckedFunction(DefinedFunction):
@@ -66,46 +65,46 @@
     cfg: CheckedCFG
 
 
 def check_global_func_def(func: DefinedFunction, globals: Globals) -> CheckedFunction:
     """Type checks a top-level function definition."""
     func_def = func.defined_at
     args = func_def.args.args
-    returns_none = isinstance(func.ty.returns, NoneType)
-    assert func.ty.arg_names is not None
+    returns_none = isinstance(func.ty.output, NoneType)
+    assert func.ty.input_names is not None
 
     cfg = CFGBuilder().build(func_def.body, returns_none, globals)
     inputs = [
         Variable(x, ty, loc, None)
-        for x, ty, loc in zip(func.ty.arg_names, func.ty.args, args)
+        for x, ty, loc in zip(func.ty.input_names, func.ty.inputs, args)
     ]
-    cfg = check_cfg(cfg, inputs, func.ty.returns, globals)
+    cfg = check_cfg(cfg, inputs, func.ty.output, globals)
     return CheckedFunction(func_def.name, func.ty, func_def, None, cfg)
 
 
 def check_nested_func_def(
     func_def: NestedFunctionDef, bb: BB, ctx: Context
 ) -> CheckedNestedFunctionDef:
     """Type checks a local (nested) function definition."""
     func_ty = check_signature(func_def, ctx.globals)
-    assert func_ty.arg_names is not None
+    assert func_ty.input_names is not None
 
     # We've already built the CFG for this function while building the CFG of the
     # enclosing function
     cfg = func_def.cfg
 
     # Find captured variables
     parent_cfg = bb.containing_cfg
-    def_ass_before = set(func_ty.arg_names) | ctx.locals.keys()
+    def_ass_before = set(func_ty.input_names) | ctx.locals.keys()
     maybe_ass_before = def_ass_before | parent_cfg.maybe_ass_before[bb]
     cfg.analyze(def_ass_before, maybe_ass_before)
     captured = {
         x: ctx.locals[x]
         for x in cfg.live_before[cfg.entry_bb]
-        if x not in func_ty.arg_names and x in ctx.locals
+        if x not in func_ty.input_names and x in ctx.locals
     }
 
     # Captured variables may not be linear
     for v in captured.values():
         if v.ty.linear:
             x = v.name
             using_bb = cfg.live_before[cfg.entry_bb][x]
@@ -127,15 +126,15 @@
                     bb.vars.assigned[x],
                     [v.defined_at],
                 )
 
     # Construct inputs for checking the body CFG
     inputs = list(captured.values()) + [
         Variable(x, ty, func_def.args.args[i], None)
-        for i, (x, ty) in enumerate(zip(func_ty.arg_names, func_ty.args))
+        for i, (x, ty) in enumerate(zip(func_ty.input_names, func_ty.inputs))
     ]
     globals = ctx.globals
 
     # Check if the body contains a free (recursive) occurrence of the function name.
     # By checking if the name is free at the entry BB, we avoid false positives when
     # a user shadows the name with a local variable
     if func_def.name in cfg.live_before[cfg.entry_bb]:
@@ -144,15 +143,15 @@
             func = DefinedFunction(func_def.name, func_ty, func_def, None)
             globals = ctx.globals | Globals({func_def.name: func}, {}, {}, {})
 
         else:
             # Otherwise, we treat it like a local name
             inputs.append(Variable(func_def.name, func_def.ty, func_def, None))
 
-    checked_cfg = check_cfg(cfg, inputs, func_ty.returns, globals)
+    checked_cfg = check_cfg(cfg, inputs, func_ty.output, globals)
     checked_def = CheckedNestedFunctionDef(
         checked_cfg,
         func_ty,
         captured,
         name=func_def.name,
         args=func_def.args,
         body=func_def.body,
@@ -184,24 +183,24 @@
             raise GuppyError(
                 "Return type must be annotated. Try adding a `-> None` annotation.",
                 func_def,
             )
         raise GuppyError("Return type must be annotated", func_def)
 
     # TODO: Prepopulate mapping when using Python 3.12 style generic functions
-    type_var_mapping: dict[str, BoundTypeVar] = {}
-    arg_tys = []
-    arg_names = []
-    for _i, arg in enumerate(func_def.args.args):
-        if arg.annotation is None:
-            raise GuppyError("Argument type must be annotated", arg)
-        ty = type_from_ast(arg.annotation, globals, type_var_mapping)
-        arg_tys.append(ty)
-        arg_names.append(arg.arg)
-
+    type_var_mapping: dict[str, "Parameter"] = {}
+    input_tys = []
+    input_names = []
+    for inp in func_def.args.args:
+        if inp.annotation is None:
+            raise GuppyError("Argument type must be annotated", inp)
+        ty = type_from_ast(inp.annotation, globals, type_var_mapping)
+        input_tys.append(ty)
+        input_names.append(inp.arg)
     ret_type = type_from_ast(func_def.returns, globals, type_var_mapping)
+
     return FunctionType(
-        arg_tys,
+        input_tys,
         ret_type,
-        arg_names,
+        input_names,
         sorted(type_var_mapping.values(), key=lambda v: v.idx),
     )
```

### Comparing `guppylang-0.1.0/guppylang/checker/stmt_checker.py` & `guppylang-0.2.0/guppylang/checker/stmt_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,43 +12,45 @@
 from collections.abc import Sequence
 
 from guppylang.ast_util import AstVisitor, with_loc
 from guppylang.cfg.bb import BB, BBStatement
 from guppylang.checker.core import Context, Variable
 from guppylang.checker.expr_checker import ExprChecker, ExprSynthesizer
 from guppylang.error import GuppyError, GuppyTypeError, InternalGuppyError
-from guppylang.gtypes import GuppyType, NoneType, Subst, TupleType, type_from_ast
 from guppylang.nodes import NestedFunctionDef
+from guppylang.tys.parsing import type_from_ast
+from guppylang.tys.subst import Subst
+from guppylang.tys.ty import NoneType, TupleType, Type
 
 
 class StmtChecker(AstVisitor[BBStatement]):
     ctx: Context
     bb: BB | None
-    return_ty: GuppyType | None
+    return_ty: Type | None
 
     def __init__(
-        self, ctx: Context, bb: BB | None = None, return_ty: GuppyType | None = None
+        self, ctx: Context, bb: BB | None = None, return_ty: Type | None = None
     ) -> None:
         assert not return_ty or not return_ty.unsolved_vars
         self.ctx = ctx
         self.bb = bb
         self.return_ty = return_ty
 
     def check_stmts(self, stmts: Sequence[BBStatement]) -> list[BBStatement]:
         return [self.visit(s) for s in stmts]
 
-    def _synth_expr(self, node: ast.expr) -> tuple[ast.expr, GuppyType]:
+    def _synth_expr(self, node: ast.expr) -> tuple[ast.expr, Type]:
         return ExprSynthesizer(self.ctx).synthesize(node)
 
     def _check_expr(
-        self, node: ast.expr, ty: GuppyType, kind: str = "expression"
+        self, node: ast.expr, ty: Type, kind: str = "expression"
     ) -> tuple[ast.expr, Subst]:
         return ExprChecker(self.ctx).check(node, ty, kind)
 
-    def _check_assign(self, lhs: ast.expr, ty: GuppyType, node: ast.stmt) -> None:
+    def _check_assign(self, lhs: ast.expr, ty: Type, node: ast.stmt) -> None:
         """Helper function to check assignments with patterns."""
         match lhs:
             # Easiest case is if the LHS pattern is a single variable.
             case ast.Name(id=x):
                 # Check if we override an unused linear variable
                 if x in self.ctx.locals:
                     var = self.ctx.locals[x]
```

### Comparing `guppylang-0.1.0/guppylang/compiler/cfg_compiler.py` & `guppylang-0.2.0/guppylang/compiler/cfg_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     DFContainer,
     PortVariable,
     is_return_var,
     return_var,
 )
 from guppylang.compiler.expr_compiler import ExprCompiler
 from guppylang.compiler.stmt_compiler import StmtCompiler
-from guppylang.gtypes import SumType, TupleType, type_to_row
 from guppylang.hugr.hugr import CFNode, Hugr, Node, OutPortV
+from guppylang.tys.definition import is_bool_type
+from guppylang.tys.ty import SumType, TupleType, type_to_row
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 
 def compile_cfg(
     cfg: CheckedCFG, graph: Hugr, parent: Node, globals: CompiledGlobals
@@ -131,16 +132,18 @@
     graph: Hugr, unit_sum: OutPortV, output_vars: list[VarRow], dfg: DFContainer
 ) -> OutPortV:
     """Selects an output based on a TupleSum.
 
     Given `unit_sum: Sum((), (), ...)` and output variable sets `#s1, #s2, ...`,
     constructs a TupleSum value of type `Sum(Tuple(#s1), Tuple(#s2), ...)`.
     """
-    assert isinstance(unit_sum.ty, SumType)
-    assert len(unit_sum.ty.element_types) == len(output_vars)
+    assert isinstance(unit_sum.ty, SumType) or is_bool_type(unit_sum.ty)
+    assert len(output_vars) == (
+        len(unit_sum.ty.element_types) if isinstance(unit_sum.ty, SumType) else 2
+    )
     tuples = [
         graph.add_make_tuple(
             inputs=[dfg[v.name].port for v in sort_vars(vs) if v.name in dfg],
             parent=dfg.node,
         ).out_port(0)
         for vs in output_vars
     ]
```

### Comparing `guppylang-0.1.0/guppylang/compiler/core.py` & `guppylang-0.2.0/guppylang/compiler/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from dataclasses import dataclass
 
 from guppylang.ast_util import AstNode
 from guppylang.checker.core import CallableVariable, Variable
-from guppylang.gtypes import FunctionType, Inst
 from guppylang.hugr.hugr import DFContainingNode, Hugr, OutPortV
+from guppylang.tys.subst import Inst
+from guppylang.tys.ty import FunctionType
 
 
 @dataclass
 class PortVariable(Variable):
     """Represents a local variable in a dataflow graph.
 
     Local variables are associated with a port in the Hugr.
```

### Comparing `guppylang-0.1.0/guppylang/compiler/expr_compiler.py` & `guppylang-0.2.0/guppylang/compiler/expr_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,35 @@
 from guppylang.compiler.core import (
     CompiledFunction,
     CompilerBase,
     DFContainer,
     PortVariable,
 )
 from guppylang.error import GuppyError, InternalGuppyError
-from guppylang.gtypes import (
-    BoolType,
-    BoundTypeVar,
-    FunctionType,
-    Inst,
-    NoneType,
-    TupleType,
-    type_to_row,
-)
 from guppylang.hugr import ops, val
 from guppylang.hugr.hugr import DFContainingNode, OutPortV, VNode
 from guppylang.nodes import (
     DesugaredGenerator,
     DesugaredListComp,
     GlobalCall,
     GlobalName,
     LocalCall,
     LocalName,
     TypeApply,
 )
+from guppylang.tys.definition import bool_type, get_element_type, is_list_type
+from guppylang.tys.subst import Inst
+from guppylang.tys.ty import (
+    BoundTypeVar,
+    FunctionType,
+    NoneType,
+    TupleType,
+    Type,
+    type_to_row,
+)
 
 
 class ExprCompiler(CompilerBase, AstVisitor[OutPortV]):
     """A compiler from guppylang expressions to Hugr."""
 
     dfg: DFContainer
 
@@ -132,15 +133,15 @@
         with self._new_case(inputs, inputs, cond_node):
             yield
         # Update the DFG with the outputs from the Conditional node
         for name in inputs:
             self.dfg[name.id].port = cond_node.add_out_port(get_type(name))
 
     def visit_Constant(self, node: ast.Constant) -> OutPortV:
-        if value := python_value_to_hugr(node.value):
+        if value := python_value_to_hugr(node.value, get_type(node)):
             const = self.graph.add_constant(value, get_type(node)).out_port(0)
             return self.graph.add_load_constant(const).out_port(0)
         raise InternalGuppyError("Unsupported constant expression in compiler")
 
     def visit_LocalName(self, node: LocalName) -> OutPortV:
         return self.dfg[node.id].port
 
@@ -169,15 +170,15 @@
 
     def visit_LocalCall(self, node: LocalCall) -> OutPortV:
         func = self.visit(node.func)
         assert isinstance(func.ty, FunctionType)
 
         args = [self.visit(arg) for arg in node.args]
         call = self.graph.add_indirect_call(func, args)
-        rets = [call.out_port(i) for i in range(len(type_to_row(func.ty.returns)))]
+        rets = [call.out_port(i) for i in range(len(type_to_row(func.ty.output)))]
         return self._pack_returns(rets)
 
     def visit_GlobalCall(self, node: GlobalCall) -> OutPortV:
         func = self.globals[node.func.name]
         assert isinstance(func, CompiledFunction)
 
         args = [self.visit(arg) for arg in node.args]
@@ -188,39 +189,39 @@
 
     def visit_Call(self, node: ast.Call) -> OutPortV:
         raise InternalGuppyError("Node should have been removed during type checking.")
 
     def visit_TypeApply(self, node: TypeApply) -> OutPortV:
         func = self.visit(node.value)
         assert isinstance(func.ty, FunctionType)
-        ta = self.graph.add_type_apply(func, node.tys, self.dfg.node).out_port(0)
+        ta = self.graph.add_type_apply(func, node.inst, self.dfg.node).out_port(0)
 
         # We have to be very careful here: If we instantiate `foo: forall T. T -> T`
         # with a tuple type `tuple[A, B]`, we get the type `tuple[A, B] -> tuple[A, B]`.
         # Normally, this would be represented in Hugr as a function with two output
         # ports types A and B. However, when TypeApplying `foo`, we actually get a
         # function with a single output port typed `tuple[A, B]`.
         # TODO: We would need to do manual monomorphisation in that case to obtain a
         #  function that returns two ports as expected
-        if instantiation_needs_unpacking(func.ty, node.tys):
+        if instantiation_needs_unpacking(func.ty, node.inst):
             raise GuppyError(
                 "Generic function instantiations returning rows are not supported yet",
                 node,
             )
 
         return ta
 
     def visit_UnaryOp(self, node: ast.UnaryOp) -> OutPortV:
         # The only case that is not desugared by the type checker is the `not` operation
         # since it is not implemented via a dunder method
         if isinstance(node.op, ast.Not):
             arg = self.visit(node.operand)
             return self.graph.add_node(
                 ops.CustomOp(extension="logic", op_name="Not", args=[]), inputs=[arg]
-            ).add_out_port(BoolType())
+            ).add_out_port(bool_type())
 
         raise InternalGuppyError("Node should have been removed during type checking.")
 
     def visit_DesugaredListComp(self, node: DesugaredListComp) -> OutPortV:
         from guppylang.compiler.stmt_compiler import StmtCompiler
 
         compiler = StmtCompiler(self.graph, self.globals)
@@ -285,39 +286,54 @@
 def expr_to_row(expr: ast.expr) -> list[ast.expr]:
     """Turns an expression into a row expressions by unpacking top-level tuples."""
     return expr.elts if isinstance(expr, ast.Tuple) else [expr]
 
 
 def instantiation_needs_unpacking(func_ty: FunctionType, inst: Inst) -> bool:
     """Checks if instantiating a polymorphic makes it return a row."""
-    if isinstance(func_ty.returns, BoundTypeVar):
-        return_ty = inst[func_ty.returns.idx]
+    if isinstance(func_ty.output, BoundTypeVar):
+        return_ty = inst[func_ty.output.idx]
         return isinstance(return_ty, TupleType | NoneType)
     return False
 
 
-def python_value_to_hugr(v: Any) -> val.Value | None:
+def python_value_to_hugr(v: Any, exp_ty: Type) -> val.Value | None:
     """Turns a Python value into a Hugr value.
 
     Returns None if the Python value cannot be represented in Guppy.
     """
-    from guppylang.prelude._internal import bool_value, float_value, int_value
+    from guppylang.prelude._internal import (
+        bool_value,
+        float_value,
+        int_value,
+        list_value,
+    )
 
     match v:
         case bool():
             return bool_value(v)
         case int():
             return int_value(v)
         case float():
             return float_value(v)
         case tuple(elts):
-            vs = [python_value_to_hugr(elt) for elt in elts]
+            assert isinstance(exp_ty, TupleType)
+            vs = [
+                python_value_to_hugr(elt, ty)
+                for elt, ty in zip(elts, exp_ty.element_types)
+            ]
             if any(value is None for value in vs):
                 return None
             return val.Tuple(vs=vs)
+        case list(elts):
+            assert is_list_type(exp_ty)
+            return list_value(
+                [python_value_to_hugr(elt, get_element_type(exp_ty)) for elt in elts],
+                get_element_type(exp_ty).to_hugr(),
+            )
         case _:
             # Pytket conversion is an optional feature
             try:
                 import pytket
 
                 if isinstance(v, pytket.circuit.Circuit):
                     from tket2.circuit import (  # type: ignore[import-untyped, import-not-found, unused-ignore]
```

### Comparing `guppylang-0.1.0/guppylang/compiler/func_compiler.py` & `guppylang-0.2.0/guppylang/compiler/func_compiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from guppylang.compiler.cfg_compiler import compile_cfg
 from guppylang.compiler.core import (
     CompiledFunction,
     CompiledGlobals,
     DFContainer,
     PortVariable,
 )
-from guppylang.gtypes import FunctionType, Inst, type_to_row
 from guppylang.hugr.hugr import DFContainingVNode, Hugr, OutPortV
 from guppylang.nodes import CheckedNestedFunctionDef
+from guppylang.tys.subst import Inst
+from guppylang.tys.ty import FunctionType, type_to_row
 
 
 @dataclass
 class CompiledFunctionDef(DefinedFunction, CompiledFunction):
     node: DFContainingVNode
 
     def load(
@@ -36,25 +37,25 @@
         #   avoid loading the function to manually add a `TypeApply`
         if type_args:
             func = graph.add_load_constant(self.node.out_port(0), dfg.node)
             func = graph.add_type_apply(func.out_port(0), type_args, dfg.node)
             call = graph.add_indirect_call(func.out_port(0), args, dfg.node)
         else:
             call = graph.add_call(self.node.out_port(0), args, dfg.node)
-        return [call.out_port(i) for i in range(len(type_to_row(self.ty.returns)))]
+        return [call.out_port(i) for i in range(len(type_to_row(self.ty.output)))]
 
 
 def compile_global_func_def(
     func: CheckedFunction,
     def_node: DFContainingVNode,
     graph: Hugr,
     globals: CompiledGlobals,
 ) -> CompiledFunctionDef:
     """Compiles a top-level function definition to Hugr."""
-    _, ports = graph.add_input_with_ports(list(func.ty.args), def_node)
+    _, ports = graph.add_input_with_ports(list(func.ty.inputs), def_node)
     cfg_node = graph.add_cfg(def_node, ports)
     compile_cfg(func.cfg, graph, cfg_node, globals)
 
     # Add output node for the cfg
     graph.add_output(
         inputs=[cfg_node.add_out_port(ty) for ty in type_to_row(func.cfg.output_ty)],
         parent=def_node,
@@ -66,28 +67,30 @@
 def compile_local_func_def(
     func: CheckedNestedFunctionDef,
     dfg: DFContainer,
     graph: Hugr,
     globals: CompiledGlobals,
 ) -> PortVariable:
     """Compiles a local (nested) function definition to Hugr."""
-    assert func.ty.arg_names is not None
+    assert func.ty.input_names is not None
 
     # Pick an order for the captured variables
     captured = list(func.captured.values())
 
     # Prepend captured variables to the function arguments
     closure_ty = FunctionType(
-        [v.ty for v in captured] + list(func.ty.args),
-        func.ty.returns,
-        [v.name for v in captured] + list(func.ty.arg_names),
+        [v.ty for v in captured] + list(func.ty.inputs),
+        func.ty.output,
+        [v.name for v in captured] + list(func.ty.input_names),
     )
 
     def_node = graph.add_def(closure_ty, dfg.node, func.name)
-    def_input, input_ports = graph.add_input_with_ports(list(closure_ty.args), def_node)
+    def_input, input_ports = graph.add_input_with_ports(
+        list(closure_ty.inputs), def_node
+    )
 
     # If we have captured variables and the body contains a recursive occurrence of
     # the function itself, then we provide the partially applied function as a local
     # variable
     if len(captured) > 0 and func.name in func.cfg.live_before[func.cfg.entry_bb]:
         loaded = graph.add_load_constant(def_node.out_port(0), def_node).out_port(0)
         partial = graph.add_partial(
```

### Comparing `guppylang-0.1.0/guppylang/compiler/stmt_compiler.py` & `guppylang-0.2.0/guppylang/compiler/stmt_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     CompilerBase,
     DFContainer,
     PortVariable,
     return_var,
 )
 from guppylang.compiler.expr_compiler import ExprCompiler
 from guppylang.error import InternalGuppyError
-from guppylang.gtypes import TupleType
 from guppylang.hugr.hugr import Hugr, OutPortV
 from guppylang.nodes import CheckedNestedFunctionDef
+from guppylang.tys.ty import TupleType
 
 
 class StmtCompiler(CompilerBase, AstVisitor[None]):
     """A compiler for Guppy statements to Hugr"""
 
     expr_compiler: ExprCompiler
```

### Comparing `guppylang-0.1.0/guppylang/custom.py` & `guppylang-0.2.0/guppylang/custom.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 from abc import ABC, abstractmethod
 
 from guppylang.ast_util import AstNode, get_type, with_loc, with_type
 from guppylang.checker.core import Context, Globals
 from guppylang.checker.expr_checker import check_call, synthesize_call
 from guppylang.checker.func_checker import check_signature
 from guppylang.compiler.core import CompiledFunction, CompiledGlobals, DFContainer
-from guppylang.error import (
-    GuppyError,
-    InternalGuppyError,
-    UnknownFunctionType,
-)
-from guppylang.gtypes import FunctionType, GuppyType, Inst, Subst, type_to_row
+from guppylang.error import GuppyError, InternalGuppyError
 from guppylang.hugr import ops
 from guppylang.hugr.hugr import DFContainingVNode, Hugr, Node, OutPortV
 from guppylang.nodes import GlobalCall
+from guppylang.tys.subst import Inst, Subst
+from guppylang.tys.ty import FunctionType, NoneType, Type, type_to_row
 
 
 class CustomFunction(CompiledFunction):
     """A function whose type checking and compilation behaviour can be customised."""
 
     defined_at: ast.FunctionDef | None
 
@@ -49,15 +46,18 @@
         self.used = None
         self._ty = ty
         self._defined = {}
 
     @property  # type: ignore[override]
     def ty(self) -> FunctionType:
         if self._ty is None:
-            return UnknownFunctionType()
+            # If we don't have a specified type, then the extension writer has to
+            # provide their own type-checking code. Therefore, it doesn't matter which
+            # type we return here since it will never be inspected.
+            return FunctionType([], NoneType())
         return self._ty
 
     @ty.setter
     def ty(self, ty: FunctionType) -> None:
         self._ty = ty
 
     def check_type(self, globals: Globals) -> None:
@@ -79,23 +79,23 @@
         except GuppyError:
             # We can ignore the error if a custom call checker is provided and the
             # function may not be used as a higher-order value
             if self.call_checker is None or self.higher_order_value:
                 raise
 
     def check_call(
-        self, args: list[ast.expr], ty: GuppyType, node: AstNode, ctx: Context
+        self, args: list[ast.expr], ty: Type, node: AstNode, ctx: Context
     ) -> tuple[ast.expr, Subst]:
         self.call_checker._setup(ctx, node, self)
         new_node, subst = self.call_checker.check(args, ty)
         return with_type(ty, with_loc(node, new_node)), subst
 
     def synthesize_call(
         self, args: list[ast.expr], node: AstNode, ctx: "Context"
-    ) -> tuple[ast.expr, GuppyType]:
+    ) -> tuple[ast.expr, Type]:
         self.call_checker._setup(ctx, node, self)
         new_node, ty = self.call_checker.synthesize(args)
         return with_type(ty, with_loc(node, new_node)), ty
 
     def compile_call(
         self,
         args: list[OutPortV],
@@ -119,15 +119,15 @@
         """
         if self._ty is None:
             raise GuppyError(
                 "This function does not support usage in a higher-order context",
                 node,
             )
 
-        if self._ty.quantified:
+        if self._ty.parametrized:
             raise InternalGuppyError(
                 "Can't yet generate higher-order versions of custom functions. This "
                 "requires generic function *definitions*"
             )
 
         # Find the module node by walking up the hierarchy
         module: Node = dfg.node
@@ -139,15 +139,15 @@
             module = module.parent
 
         # If the function has not yet been loaded in this module, we first have to
         # define it. We create a `FunctionDef` that takes some inputs, compiles a call
         # to the function, and returns the results.
         if module not in self._defined:
             def_node = graph.add_def(self.ty, module, self.name)
-            _, inp_ports = graph.add_input_with_ports(list(self.ty.args), def_node)
+            _, inp_ports = graph.add_input_with_ports(list(self.ty.inputs), def_node)
             returns = self.compile_call(
                 inp_ports, [], DFContainer(def_node, {}), graph, globals, node
             )
             graph.add_output(returns, parent=def_node)
             self._defined[module] = def_node
 
         # Finally, load the function into the local DFG
@@ -165,22 +165,22 @@
 
     def _setup(self, ctx: Context, node: AstNode, func: CustomFunction) -> None:
         self.ctx = ctx
         self.node = node
         self.func = func
 
     @abstractmethod
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         """Checks the return value against a given type.
 
         Returns a (possibly) transformed and annotated AST node for the call.
         """
 
     @abstractmethod
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         """Synthesizes a type for the return value of a call.
 
         Also returns a (possibly) transformed and annotated argument list.
         """
 
 
 class CustomCallCompiler(ABC):
@@ -210,20 +210,20 @@
     def compile(self, args: list[OutPortV]) -> list[OutPortV]:
         """Compiles a custom function call and returns the resulting ports."""
 
 
 class DefaultCallChecker(CustomCallChecker):
     """Checks function calls by comparing to a type signature."""
 
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         # Use default implementation from the expression checker
         args, subst, inst = check_call(self.func.ty, args, ty, self.node, self.ctx)
         return GlobalCall(func=self.func, args=args, type_args=inst), subst
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         # Use default implementation from the expression checker
         args, ty, inst = synthesize_call(self.func.ty, args, self.node, self.ctx)
         return GlobalCall(func=self.func, args=args, type_args=inst), ty
 
 
 class DefaultCallCompiler(CustomCallCompiler):
     """Call compiler that invokes the regular expression compiler."""
```

### Comparing `guppylang-0.1.0/guppylang/declared.py` & `guppylang-0.2.0/guppylang/declared.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 from guppylang.ast_util import AstNode, has_empty_body, with_loc
 from guppylang.checker.core import Context, Globals
 from guppylang.checker.expr_checker import check_call, synthesize_call
 from guppylang.checker.func_checker import check_signature
 from guppylang.compiler.core import CompiledFunction, CompiledGlobals, DFContainer
 from guppylang.error import GuppyError
-from guppylang.gtypes import GuppyType, Inst, Subst, type_to_row
 from guppylang.hugr.hugr import Hugr, Node, OutPortV, VNode
 from guppylang.nodes import GlobalCall
+from guppylang.tys.subst import Inst, Subst
+from guppylang.tys.ty import Type, type_to_row
 
 
 @dataclass
 class DeclaredFunction(CompiledFunction):
     """A user-declared function that compiles to a Hugr function declaration."""
 
     node: VNode | None = None
@@ -26,23 +27,23 @@
         if not has_empty_body(func_def):
             raise GuppyError(
                 "Body of function declaration must be empty", func_def.body[0]
             )
         return DeclaredFunction(name, ty, func_def, None)
 
     def check_call(
-        self, args: list[ast.expr], ty: GuppyType, node: AstNode, ctx: Context
+        self, args: list[ast.expr], ty: Type, node: AstNode, ctx: Context
     ) -> tuple[ast.expr, Subst]:
         # Use default implementation from the expression checker
         args, subst, inst = check_call(self.ty, args, ty, node, ctx)
         return with_loc(node, GlobalCall(func=self, args=args, type_args=inst)), subst
 
     def synthesize_call(
         self, args: list[ast.expr], node: AstNode, ctx: Context
-    ) -> tuple[GlobalCall, GuppyType]:
+    ) -> tuple[GlobalCall, Type]:
         # Use default implementation from the expression checker
         args, ty, inst = synthesize_call(self.ty, args, node, ctx)
         return with_loc(node, GlobalCall(func=self, args=args, type_args=inst)), ty
 
     def add_to_graph(self, graph: Hugr, parent: Node) -> None:
         self.node = graph.add_declare(self.ty, parent, self.name)
 
@@ -66,8 +67,8 @@
         #   avoid loading the function to manually add a `TypeApply`
         if type_args:
             func = graph.add_load_constant(self.node.out_port(0), dfg.node)
             func = graph.add_type_apply(func.out_port(0), type_args, dfg.node)
             call = graph.add_indirect_call(func.out_port(0), args, dfg.node)
         else:
             call = graph.add_call(self.node.out_port(0), args, dfg.node)
-        return [call.out_port(i) for i in range(len(type_to_row(self.ty.returns)))]
+        return [call.out_port(i) for i in range(len(type_to_row(self.ty.output)))]
```

### Comparing `guppylang-0.1.0/guppylang/decorator.py` & `guppylang-0.2.0/guppylang/decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import functools
 import inspect
-from collections.abc import Callable, Iterator, Sequence
+from collections.abc import Callable
 from dataclasses import dataclass
 from pathlib import Path
 from types import ModuleType
-from typing import Any, ClassVar, TypeVar
+from typing import Any, TypeVar
 
-from guppylang.ast_util import AstNode, has_empty_body
+from guppylang.ast_util import has_empty_body
 from guppylang.custom import (
     CustomCallChecker,
     CustomCallCompiler,
     CustomFunction,
     DefaultCallChecker,
     DefaultCallCompiler,
     OpCompiler,
 )
 from guppylang.error import GuppyError, MissingModuleError, pretty_errors
-from guppylang.gtypes import GuppyType, TypeTransformer
 from guppylang.hugr import ops, tys
 from guppylang.hugr.hugr import Hugr
 from guppylang.module import GuppyModule, PyFunc, parse_py_func
+from guppylang.tys.definition import OpaqueTypeDef, TypeDef
 
 FuncDecorator = Callable[[PyFunc], PyFunc | Hugr]
 CustomFuncDecorator = Callable[[PyFunc], CustomFunction]
 ClassDecorator = Callable[[type], type]
 
 
 @dataclass(frozen=True)
@@ -109,20 +109,20 @@
                     module = inspect.getmodule(s.frame)
                     break
             else:
                 raise GuppyError("Could not find a caller for the `@guppy` decorator")
         return ModuleIdentifier(Path(filename), module)
 
     @pretty_errors
-    def extend_type(self, module: GuppyModule, ty: type[GuppyType]) -> ClassDecorator:
+    def extend_type(self, module: GuppyModule, defn: TypeDef) -> ClassDecorator:
         """Decorator to add new instance functions to a type."""
         module._instance_func_buffer = {}
 
         def dec(c: type) -> type:
-            module._register_buffered_instance_funcs(ty)
+            module._register_buffered_instance_funcs(defn)
             return c
 
         return dec
 
     @pretty_errors
     def type(
         self,
@@ -138,56 +138,17 @@
         marked as linear. All `@guppy` annotated functions on the class are turned into
         instance functions.
         """
         module._instance_func_buffer = {}
 
         def dec(c: type) -> type:
             _name = name or c.__name__
-
-            @dataclass(frozen=True)
-            class NewType(GuppyType):
-                args: Sequence[GuppyType]
-                name: ClassVar[str] = _name
-
-                @staticmethod
-                def build(*args: GuppyType, node: AstNode | None = None) -> "GuppyType":
-                    # At the moment, custom types don't support type arguments.
-                    if len(args) > 0:
-                        raise GuppyError(
-                            f"Type `{_name}` does not accept type parameters.", node
-                        )
-                    return NewType([])
-
-                @property
-                def type_args(self) -> Iterator[GuppyType]:
-                    return iter(self.args)
-
-                @property
-                def linear(self) -> bool:
-                    return linear
-
-                def to_hugr(self) -> tys.Type:
-                    return hugr_ty
-
-                def hugr_bound(self) -> tys.TypeBound:
-                    return bound or super().hugr_bound()
-
-                def transform(self, transformer: TypeTransformer) -> GuppyType:
-                    return transformer.transform(self) or NewType(
-                        [ty.transform(transformer) for ty in self.args]
-                    )
-
-                def __str__(self) -> str:
-                    return _name
-
-            NewType.__name__ = name
-            NewType.__qualname__ = _name
-            module.register_type(_name, NewType)
-            module._register_buffered_instance_funcs(NewType)
-            c._guppy_type = NewType  # type: ignore[attr-defined]
+            defn = OpaqueTypeDef(_name, [], linear, lambda _: hugr_ty, bound)
+            module.register_type(_name, defn)
+            module._register_buffered_instance_funcs(defn)
             return c
 
         return dec
 
     @pretty_errors
     def type_var(self, module: GuppyModule, name: str, linear: bool = False) -> TypeVar:
         """Creates a new type variable in a module."""
```

### Comparing `guppylang-0.1.0/guppylang/error.py` & `guppylang-0.2.0/guppylang/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import ast
 import functools
+import os
 import sys
 import textwrap
-from collections.abc import Callable, Sequence
+from collections.abc import Callable, Iterator, Sequence
+from contextlib import contextmanager
 from dataclasses import dataclass, field
+from types import TracebackType
 from typing import Any, TypeVar, cast
 
 from guppylang.ast_util import AstNode, get_file, get_line_offset, get_source
-from guppylang.gtypes import BoundTypeVar, ExistentialTypeVar, FunctionType, GuppyType
-from guppylang.hugr.hugr import Node, OutPortV
-
-# Whether the interpreter should exit when a Guppy error occurs
-EXIT_ON_ERROR: bool = True
 
 
 @dataclass(frozen=True)
 class SourceLoc:
     """A source location associated with an AST node.
 
     This class translates the location data provided by the ast module into a location
@@ -80,64 +78,24 @@
     """Special Guppy exception for operations that require a guppy module."""
 
 
 class InternalGuppyError(Exception):
     """Exception for internal problems during compilation."""
 
 
-class UndefinedPort(OutPortV):
-    """Dummy port for undefined variables.
-
-    Raises an `InternalGuppyError` if one tries to access one of its properties.
-    """
-
-    def __init__(self, ty: GuppyType):
-        self._ty = ty
-
-    @property
-    def ty(self) -> GuppyType:
-        return self._ty
-
-    @property
-    def node(self) -> Node:
-        raise InternalGuppyError("Tried to access undefined Port")
-
-    @property
-    def offset(self) -> int:
-        raise InternalGuppyError("Tried to access undefined Port")
-
-
-class UnknownFunctionType(FunctionType):
-    """Dummy function type for custom functions without an expressible type.
-
-    Raises an `InternalGuppyError` if one tries to access one of its members.
-    """
+ExceptHook = Callable[[type[BaseException], BaseException, TracebackType | None], Any]
 
-    def __init__(self) -> None:
-        pass
 
-    @property
-    def args(self) -> Sequence[GuppyType]:
-        raise InternalGuppyError("Tried to access unknown function type")
-
-    @property
-    def returns(self) -> GuppyType:
-        raise InternalGuppyError("Tried to access unknown function type")
-
-    @property
-    def args_names(self) -> Sequence[str] | None:
-        raise InternalGuppyError("Tried to access unknown function type")
-
-    @property
-    def quantified(self) -> Sequence[BoundTypeVar]:
-        raise InternalGuppyError("Tried to access unknown function type")
-
-    @property
-    def unsolved_vars(self) -> set[ExistentialTypeVar]:
-        return set()
+@contextmanager
+def exception_hook(hook: ExceptHook) -> Iterator[None]:
+    """Sets a custom `excepthook` for the scope of a 'with' block."""
+    old_hook = sys.excepthook
+    sys.excepthook = hook
+    yield
+    sys.excepthook = old_hook
 
 
 def format_source_location(
     loc: ast.AST,
     num_lines: int = 3,
     indent: int = 4,
 ) -> str:
@@ -165,31 +123,52 @@
 
 FuncT = TypeVar("FuncT", bound=Callable[..., Any])
 
 
 def pretty_errors(f: FuncT) -> FuncT:
     """Decorator to print custom error banners when a `GuppyError` occurs."""
 
+    def hook(
+        excty: type[BaseException], err: BaseException, traceback: TracebackType | None
+    ) -> None:
+        """Custom `excepthook` that intercepts `GuppyExceptions` for pretty printing."""
+        # Fall back to default hook if it's not a GuppyException or we're missing an
+        # error location
+        if not isinstance(err, GuppyError) or err.location is None:
+            sys.__excepthook__(excty, err, traceback)
+            return
+
+        loc = err.location
+        file, line_offset = get_file(loc), get_line_offset(loc)
+        assert file is not None
+        assert line_offset is not None
+        line = line_offset + loc.lineno - 1
+        sys.stderr.write(
+            f"Guppy compilation failed. Error in file {file}:{line}\n\n"
+            f"{format_source_location(loc)}\n"
+            f"{err.__class__.__name__}: {err.get_msg()}\n",
+        )
+
     @functools.wraps(f)
     def pretty_errors_wrapped(*args: Any, **kwargs: Any) -> Any:
-        try:
-            return f(*args, **kwargs)
-        except GuppyError as err:
-            # Reraise if we're missing a location
-            if not err.location:
+        with exception_hook(hook):
+            try:
+                return f(*args, **kwargs)
+            except GuppyError as err:
+                # For normal usage, this `try` block is not necessary since the
+                # excepthook is automatically invoked when the exception (which is being
+                # reraised below) is not handled. However, when running tests, we have
+                # to manually invoke the hook to print the error message, since the
+                # tests always have to capture exceptions.
+                if _pytest_running():
+                    hook(type(err), err, err.__traceback__)
                 raise
-            loc = err.location
-            file, line_offset = get_file(loc), get_line_offset(loc)
-            assert file is not None
-            assert line_offset is not None
-            line = line_offset + loc.lineno - 1
-            print(  # noqa: T201
-                f"Guppy compilation failed. Error in file {file}:{line}\n\n"
-                f"{format_source_location(loc)}\n"
-                f"{err.__class__.__name__}: {err.get_msg()}",
-                file=sys.stderr,
-            )
-            if EXIT_ON_ERROR:
-                sys.exit(1)
-            return None
 
     return cast(FuncT, pretty_errors_wrapped)
+
+
+def _pytest_running() -> bool:
+    """Checks if we are currently running pytest.
+
+    See https://docs.pytest.org/en/latest/example/simple.html#pytest-current-test-environment-variable
+    """
+    return "PYTEST_CURRENT_TEST" in os.environ
```

### Comparing `guppylang-0.1.0/guppylang/gtypes.py` & `guppylang-0.2.0/guppylang/tys/ty.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,654 +1,516 @@
-import ast
-import itertools
 from abc import ABC, abstractmethod
-from collections.abc import Iterator, Sequence
+from collections.abc import Sequence
 from dataclasses import dataclass, field
-from typing import (
-    TYPE_CHECKING,
-    ClassVar,
-    Literal,
-)
+from functools import cached_property
+from typing import TYPE_CHECKING, TypeAlias, cast
 
-import guppylang.hugr.tys as tys
-from guppylang.ast_util import AstNode
+from guppylang.error import InternalGuppyError
+from guppylang.hugr import tys
+from guppylang.hugr.tys import TypeBound
+from guppylang.tys.arg import Argument, ConstArg, TypeArg
+from guppylang.tys.common import ToHugr, Transformable, Transformer, Visitor
+from guppylang.tys.const import ExistentialConstVar
+from guppylang.tys.param import Parameter
+from guppylang.tys.var import BoundVar, ExistentialVar
 
 if TYPE_CHECKING:
-    from guppylang.checker.core import Globals
-
-
-Subst = dict["ExistentialTypeVar", "GuppyType"]
-Inst = Sequence["GuppyType"]
+    from guppylang.tys.definition import OpaqueTypeDef
+    from guppylang.tys.subst import Inst, Subst
 
 
 @dataclass(frozen=True)
-class GuppyType(ABC):
-    """Base class for all Guppy types.
+class TypeBase(ToHugr[tys.Type], Transformable["Type"], ABC):
+    """Abstract base class for all Guppy types.
 
-    Note that all instances of `GuppyType` subclasses are expected to be immutable.
+    Note that all subclasses are expected to be immutable.
     """
 
-    name: ClassVar[str]
+    @cached_property
+    @abstractmethod
+    def linear(self) -> bool:
+        """Whether this type should be treated linearly."""
+
+    @cached_property
+    @abstractmethod
+    def hugr_bound(self) -> tys.TypeBound:
+        """The Hugr bound of this type, i.e. `Any`, `Copyable`, or `Equatable`.
 
-    # Cache for free variables
-    _unsolved_vars: set["ExistentialTypeVar"] = field(init=False, repr=False)
+        This needs to be specified explicitly, since opaque nonlinear types in a Hugr
+        extension could be either declared as copyable or equatable. If we don't get the
+        bound exactly right during serialisation, the Hugr validator will complain.
+        """
 
-    def __post_init__(self) -> None:
-        # Make sure that we don't have higher-rank polymorphic types
-        for arg in self.type_args:
-            if isinstance(arg, FunctionType) and arg.quantified:
-                from guppylang.error import InternalGuppyError
-
-                raise InternalGuppyError(
-                    "Tried to construct a higher-rank polymorphic type!"
-                )
-
-        # Compute free variables
-        if isinstance(self, ExistentialTypeVar):
-            vs = {self}
-        else:
-            vs = set()
-            for arg in self.type_args:
-                vs |= arg.unsolved_vars
-        object.__setattr__(self, "_unsolved_vars", vs)
+    @cached_property
+    def unsolved_vars(self) -> set[ExistentialVar]:
+        """The existential type variables contained in this type."""
+        return set()
+
+    def substitute(self, subst: "Subst") -> "Type":
+        """Substitutes existential variables in this type."""
+        from guppylang.tys.subst import Substituter
 
-    @staticmethod
-    @abstractmethod
-    def build(*args: "GuppyType", node: AstNode | None = None) -> "GuppyType":
-        pass
+        return self.transform(Substituter(subst))
 
-    @property
-    @abstractmethod
-    def type_args(self) -> Iterator["GuppyType"]:
-        pass
+    def __str__(self) -> str:
+        """Returns a human-readable representation of the type."""
+        from guppylang.tys.printing import TypePrinter
+
+        # We use a custom printer that takes care of inserting parentheses and choosing
+        # unique names
+        return TypePrinter().visit(cast(Type, self))
+
+
+@dataclass(frozen=True)
+class ParametrizedTypeBase(TypeBase, ABC):
+    """Abstract base class for types that depend on parameters.
+
+    For example, `list`, `tuple`, etc. require arguments in order to be turned into a
+    proper type.
+
+    Note that all subclasses are expected to be immutable.
+    """
+
+    args: Sequence[Argument]
+
+    def __post_init__(self) -> None:
+        # Make sure that we don't have nested generic functions
+        for arg in self.args:
+            match arg:
+                case TypeArg(ty=FunctionType(parametrized=True)):
+                    raise InternalGuppyError(
+                        "Tried to construct a higher-rank polymorphic type!"
+                    )
 
     @property
     @abstractmethod
-    def linear(self) -> bool:
-        pass
+    def intrinsically_linear(self) -> bool:
+        """Whether this type is linear, independent of the arguments.
 
-    @abstractmethod
-    def to_hugr(self) -> tys.Type:
-        pass
+        For example, a parametrized struct containing a qubit is linear, no matter what
+        the arguments are.
+        """
 
-    @abstractmethod
-    def transform(self, transformer: "TypeTransformer") -> "GuppyType":
-        pass
+    @cached_property
+    def linear(self) -> bool:
+        """Whether this type should be treated linearly."""
+        return self.intrinsically_linear or any(
+            isinstance(arg, TypeArg) and arg.ty.linear for arg in self.args
+        )
+
+    @cached_property
+    def unsolved_vars(self) -> set[ExistentialVar]:
+        """The existential type variables contained in this type."""
+        unsolved = set()
+        for arg in self.args:
+            match arg:
+                case TypeArg(ty):
+                    unsolved |= ty.unsolved_vars
+                case ConstArg(c) if isinstance(c, ExistentialConstVar):
+                    unsolved.add(c)
+        return unsolved
 
+    @cached_property
     def hugr_bound(self) -> tys.TypeBound:
+        """The Hugr bound of this type, i.e. `Any`, `Copyable`, or `Equatable`."""
         if self.linear:
             return tys.TypeBound.Any
-        return tys.TypeBound.join(*(ty.hugr_bound() for ty in self.type_args))
-
-    @property
-    def unsolved_vars(self) -> set["ExistentialTypeVar"]:
-        return self._unsolved_vars
+        return tys.TypeBound.join(
+            *(arg.ty.hugr_bound for arg in self.args if isinstance(arg, TypeArg))
+        )
 
-    def substitute(self, s: Subst) -> "GuppyType":
-        return self.transform(Substituter(s))
+    def visit(self, visitor: Visitor) -> None:
+        """Accepts a visitor on this type."""
+        if not visitor.visit(self):
+            for arg in self.args:
+                visitor.visit(arg)
 
 
 @dataclass(frozen=True)
-class BoundTypeVar(GuppyType):
-    """Bound type variable, identified with a de Bruijn index."""
+class BoundTypeVar(TypeBase, BoundVar):
+    """Bound type variable, referencing a parameter of kind `Type`.
 
-    idx: int
-    display_name: str
-    linear: bool = False
-
-    name: ClassVar[Literal["BoundTypeVar"]] = "BoundTypeVar"
-
-    @staticmethod
-    def build(*rgs: GuppyType, node: AstNode | None = None) -> GuppyType:
-        raise NotImplementedError
+    For example, in the function type `forall T. list[T] -> T` we represent `T` as a
+    `BoundTypeVar(idx=0)`.
 
-    @property
-    def type_args(self) -> Iterator["GuppyType"]:
-        return iter(())
+    A bound type variables can be instantiated with a `TypeArg` argument.
+    """
+
+    linear: bool
 
+    @cached_property
     def hugr_bound(self) -> tys.TypeBound:
-        # We shouldn't make variables equatable, since we also want to substitute types
-        # like `float`
-        return tys.TypeBound.Any if self.linear else tys.TypeBound.Copyable
+        """The Hugr bound of this type, i.e. `Any`, `Copyable`, or `Equatable`."""
+        if self.linear:
+            return TypeBound.Any
+        # We're conservative and don't require equatability for non-linear variables.
+        # This is fine since Guppy doesn't use the equatable feature anyways.
+        return TypeBound.Copyable
 
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
+    def to_hugr(self) -> tys.Type:
+        """Computes the Hugr representation of the type."""
+        return tys.Variable(i=self.idx, b=self.hugr_bound)
+
+    def visit(self, visitor: Visitor) -> None:
+        """Accepts a visitor on this type."""
+        visitor.visit(self)
+
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
         return transformer.transform(self) or self
 
     def __str__(self) -> str:
+        """Returns a human-readable representation of the type."""
         return self.display_name
 
-    def to_hugr(self) -> tys.Type:
-        return tys.Variable(i=self.idx, b=self.hugr_bound())
-
 
 @dataclass(frozen=True)
-class ExistentialTypeVar(GuppyType):
-    """Existential type variable, identified with a globally unique id.
+class ExistentialTypeVar(ExistentialVar, TypeBase):
+    """Existential type variable.
+
+    For example, the empty list literal `[]` is typed as `list[?T]` where `?T` stands
+    for an existential type variable.
 
-    Is solved during type checking.
+    During type checking we try to solve all existential type variables and substitute
+    them with concrete types.
     """
 
-    id: int
-    display_name: str
-    linear: bool = False
+    linear: bool
 
-    name: ClassVar[Literal["ExistentialTypeVar"]] = "ExistentialTypeVar"
+    @classmethod
+    def fresh(cls, display_name: str, linear: bool) -> "ExistentialTypeVar":
+        return ExistentialTypeVar(display_name, next(cls._fresh_id), linear)
 
-    _id_generator: ClassVar[Iterator[int]] = itertools.count()
+    @cached_property
+    def unsolved_vars(self) -> set[ExistentialVar]:
+        """The existential type variables contained in this type."""
+        return {self}
 
-    @classmethod
-    def new(cls, display_name: str, linear: bool) -> "ExistentialTypeVar":
-        return ExistentialTypeVar(next(cls._id_generator), display_name, linear)
+    @cached_property
+    def hugr_bound(self) -> tys.TypeBound:
+        """The Hugr bound of this type, i.e. `Any`, `Copyable`, or `Equatable`."""
+        raise InternalGuppyError(
+            "Tried to compute bound of unsolved existential type variable"
+        )
 
-    @staticmethod
-    def build(*rgs: GuppyType, node: AstNode | None = None) -> GuppyType:
-        raise NotImplementedError
+    def to_hugr(self) -> tys.Type:
+        """Computes the Hugr representation of the type."""
+        raise InternalGuppyError(
+            "Tried to convert unsolved existential type variable to Hugr"
+        )
 
-    @property
-    def type_args(self) -> Iterator["GuppyType"]:
-        return iter(())
+    def visit(self, visitor: Visitor) -> None:
+        """Accepts a visitor on this type."""
+        visitor.visit(self)
 
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
         return transformer.transform(self) or self
 
-    def __str__(self) -> str:
-        return "?" + self.display_name
 
-    def __hash__(self) -> int:
-        return self.id
+@dataclass(frozen=True)
+class NoneType(TypeBase):
+    """Type of tuples."""
+
+    linear: bool = field(default=False, init=False)
+    hugr_bound: tys.TypeBound = field(default=tys.TypeBound.Eq, init=False)
+
+    # Flag to avoid turning the type into a row when calling `type_to_row()`. This is
+    # used to make sure that type vars instantiated to Nones are not broken up into
+    # empty rows when generating a Hugr
+    preserve: bool = field(default=False, compare=False)
 
     def to_hugr(self) -> tys.Type:
-        from guppylang.error import InternalGuppyError
+        """Computes the Hugr representation of the type."""
+        return tys.TupleType(inner=[])
 
-        raise InternalGuppyError("Tried to convert free type variable to Hugr")
+    def visit(self, visitor: Visitor) -> None:
+        """Accepts a visitor on this type."""
+        visitor.visit(self)
 
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
+        return transformer.transform(self) or self
 
-@dataclass(frozen=True)
-class FunctionType(GuppyType):
-    args: Sequence[GuppyType]
-    returns: GuppyType
-    arg_names: Sequence[str] | None = field(
-        default=None,
-        compare=False,  # Argument names are not taken into account for type equality
-    )
-    quantified: Sequence[BoundTypeVar] = field(default_factory=list)
 
-    name: ClassVar[Literal["%function"]] = "%function"
-    linear = False
+@dataclass(frozen=True, init=False)
+class FunctionType(ParametrizedTypeBase):
+    """Type of (potentially generic) functions."""
+
+    inputs: Sequence["Type"]
+    output: "Type"
+    params: Sequence[Parameter]
+    input_names: Sequence[str] | None
 
-    def __str__(self) -> str:
-        prefix = (
-            "forall " + ", ".join(str(v) for v in self.quantified) + ". "
-            if self.quantified
-            else ""
-        )
-        if len(self.args) == 1:
-            [arg] = self.args
-            return prefix + f"{arg} -> {self.returns}"
-        else:
-            return (
-                prefix + f"({', '.join(str(a) for a in self.args)}) -> {self.returns}"
-            )
-
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        # Function types cannot be constructed using `build`. The type parsing code
-        # has a special case for function types.
-        raise NotImplementedError
+    args: Sequence[Argument] = field(init=False)
+    linear: bool = field(default=False, init=False)
+    intrinsically_linear: bool = field(default=False, init=False)
+    hugr_bound: tys.TypeBound = field(default=TypeBound.Copyable, init=False)
 
-    @property
-    def type_args(self) -> Iterator[GuppyType]:
-        return itertools.chain(iter(self.args), iter((self.returns,)))
+    def __init__(
+        self,
+        inputs: Sequence["Type"],
+        output: "Type",
+        input_names: Sequence[str] | None = None,
+        params: Sequence[Parameter] | None = None,
+    ) -> None:
+        # We need a custom __init__ to set the args
+        args = [TypeArg(ty) for ty in inputs]
+        args.append(TypeArg(output))
+        object.__setattr__(self, "args", args)
+        object.__setattr__(self, "inputs", inputs)
+        object.__setattr__(self, "output", output)
+        object.__setattr__(self, "input_names", input_names or [])
+        object.__setattr__(self, "params", params or [])
+
+    @property
+    def parametrized(self) -> bool:
+        """Whether the function is parametrized."""
+        return len(self.params) > 0
 
-    def to_hugr(self) -> tys.PolyFuncType:
-        ins = [t.to_hugr() for t in self.args]
-        outs = [t.to_hugr() for t in type_to_row(self.returns)]
+    def to_hugr(self) -> tys.Type:
+        """Computes the Hugr representation of the type."""
+        ins = [t.to_hugr() for t in self.inputs]
+        outs = [t.to_hugr() for t in type_to_row(self.output)]
         func_ty = tys.FunctionType(input=ins, output=outs, extension_reqs=[])
-        return tys.PolyFuncType(
-            params=[tys.TypeTypeParam(b=v.hugr_bound()) for v in self.quantified],
-            body=func_ty,
-        )
+        return tys.PolyFuncType(params=[p.to_hugr() for p in self.params], body=func_ty)
 
-    def hugr_bound(self) -> tys.TypeBound:
-        # Functions are not equatable, only copyable
-        return tys.TypeBound.Copyable
+    def visit(self, visitor: Visitor) -> None:
+        """Accepts a visitor on this type."""
+        if not visitor.visit(self):
+            for inp in self.inputs:
+                visitor.visit(inp)
+            visitor.visit(self.output)
+            for param in self.params:
+                visitor.visit(param)
 
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
         return transformer.transform(self) or FunctionType(
-            [ty.transform(transformer) for ty in self.args],
-            self.returns.transform(transformer),
-            self.arg_names,
+            [inp.transform(transformer) for inp in self.inputs],
+            self.output.transform(transformer),
+            self.input_names,
+            self.params,
         )
 
-    def instantiate(self, tys: Sequence[GuppyType]) -> "FunctionType":
-        """Instantiates quantified type variables."""
-        assert len(tys) == len(self.quantified)
+    def instantiate(self, args: "Inst") -> "FunctionType":
+        """Instantiates all function parameters with concrete types."""
+        from guppylang.tys.subst import Instantiator
+
+        assert len(args) == len(self.params)
 
         # Set the `preserve` flag for instantiated tuples and None
-        preserved_tys: list[GuppyType] = []
-        for ty in tys:
-            if isinstance(ty, TupleType):
-                ty = TupleType(ty.element_types, preserve=True)
-            elif isinstance(ty, NoneType):
-                ty = NoneType(preserve=True)
-            preserved_tys.append(ty)
+        preserved_args: list[Argument] = []
+        for arg in args:
+            if isinstance(arg, TypeArg):
+                if isinstance(arg.ty, TupleType):
+                    arg = TypeArg(TupleType(arg.ty.element_types, preserve=True))
+                elif isinstance(arg.ty, NoneType):
+                    arg = TypeArg(NoneType(preserve=True))
+            preserved_args.append(arg)
 
-        inst = Instantiator(preserved_tys)
+        inst = Instantiator(preserved_args)
         return FunctionType(
-            [ty.transform(inst) for ty in self.args],
-            self.returns.transform(inst),
-            self.arg_names,
+            [ty.transform(inst) for ty in self.inputs],
+            self.output.transform(inst),
+            self.input_names,
         )
 
-    def unquantified(self) -> tuple["FunctionType", Sequence[ExistentialTypeVar]]:
-        """Replaces all quantified variables with free type variables."""
-        inst = [
-            ExistentialTypeVar.new(v.display_name, v.linear) for v in self.quantified
-        ]
-        return self.instantiate(inst), inst
+    def unquantified(self) -> tuple["FunctionType", Sequence[ExistentialVar]]:
+        """Instantiates all parameters with existential variables."""
+        exs = [param.to_existential() for param in self.params]
+        return self.instantiate([arg for arg, _ in exs]), [var for _, var in exs]
 
 
-@dataclass(frozen=True)
-class TupleType(GuppyType):
-    element_types: Sequence[GuppyType]
+@dataclass(frozen=True, init=False)
+class TupleType(ParametrizedTypeBase):
+    """Type of tuples."""
+
+    element_types: Sequence["Type"]
 
-    # Flag to avoid turning the tuple into row when calling `type_to_row()`. This is
+    # Flag to avoid turning the tuple into a row when calling `type_to_row()`. This is
     # used to make sure that type vars instantiated to tuples are not broken up into
     # rows when generating a Hugr
     preserve: bool = field(default=False, compare=False)
 
-    name: ClassVar[Literal["tuple"]] = "tuple"
-
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        from guppylang.error import GuppyError
-
-        # TODO: Parse empty tuples via `tuple[()]`
-        if len(args) == 0:
-            raise GuppyError("Tuple type requires generic type arguments", node)
-        return TupleType(list(args))
-
-    def __str__(self) -> str:
-        return f"({', '.join(str(e) for e in self.element_types)})"
-
-    @property
-    def linear(self) -> bool:
-        return any(t.linear for t in self.element_types)
+    def __init__(self, element_types: Sequence["Type"], preserve: bool = False) -> None:
+        # We need a custom __init__ to set the args
+        args = [TypeArg(ty) for ty in element_types]
+        object.__setattr__(self, "args", args)
+        object.__setattr__(self, "element_types", element_types)
+        object.__setattr__(self, "preserve", preserve)
 
     @property
-    def type_args(self) -> Iterator[GuppyType]:
-        return iter(self.element_types)
+    def intrinsically_linear(self) -> bool:
+        return False
 
     def to_hugr(self) -> tys.Type:
-        ts = [t.to_hugr() for t in self.element_types]
-        return tys.TupleType(inner=ts)
+        """Computes the Hugr representation of the type."""
+        return tys.TupleType(inner=[ty.to_hugr() for ty in self.element_types])
 
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
         return transformer.transform(self) or TupleType(
-            [ty.transform(transformer) for ty in self.element_types]
+            [ty.transform(transformer) for ty in self.element_types], self.preserve
         )
 
 
-@dataclass(frozen=True)
-class SumType(GuppyType):
-    element_types: Sequence[GuppyType]
-
-    name: ClassVar[str] = "%tuple"
+@dataclass(frozen=True, init=False)
+class SumType(ParametrizedTypeBase):
+    """Type of sums.
 
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        # Sum types cannot be parsed and constructed using `build` since they cannot be
-        # written by the user
-        raise NotImplementedError
+    Note that this type is only used internally when constructing the Hugr. Users cannot
+    write down this type.
+    """
 
-    def __str__(self) -> str:
-        return f"Sum({', '.join(str(e) for e in self.element_types)})"
+    element_types: Sequence["Type"]
 
-    @property
-    def linear(self) -> bool:
-        return any(t.linear for t in self.element_types)
+    def __init__(self, element_types: Sequence["Type"]) -> None:
+        # We need a custom __init__ to set the args
+        args = [TypeArg(ty) for ty in element_types]
+        object.__setattr__(self, "args", args)
+        object.__setattr__(self, "element_types", element_types)
 
     @property
-    def type_args(self) -> Iterator[GuppyType]:
-        return iter(self.element_types)
+    def intrinsically_linear(self) -> bool:
+        return False
 
     def to_hugr(self) -> tys.Type:
+        """Computes the Hugr representation of the type."""
         if all(
             isinstance(e, TupleType) and len(e.element_types) == 0
             for e in self.element_types
         ):
             return tys.UnitSum(size=len(self.element_types))
         return tys.GeneralSum(row=[t.to_hugr() for t in self.element_types])
 
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
         return transformer.transform(self) or SumType(
             [ty.transform(transformer) for ty in self.element_types]
         )
 
 
 @dataclass(frozen=True)
-class ListType(GuppyType):
-    element_type: GuppyType
+class OpaqueType(ParametrizedTypeBase):
+    """Type that is directly backed by a Hugr opaque type.
 
-    name: ClassVar[Literal["list"]] = "list"
-    linear: bool = field(default=False, init=False)
-
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        from guppylang.error import GuppyError
-
-        if len(args) == 0:
-            raise GuppyError("Missing type parameter for generic type `list`", node)
-        if len(args) > 1:
-            raise GuppyError("Too many type arguments for generic type `list`", node)
-        (arg,) = args
-        if arg.linear:
-            raise GuppyError(
-                "Type `list` cannot store linear data, use `linst` instead", node
-            )
-        return ListType(arg)
-
-    def __str__(self) -> str:
-        return f"list[{self.element_type}]"
-
-    @property
-    def type_args(self) -> Iterator[GuppyType]:
-        return iter((self.element_type,))
-
-    def to_hugr(self) -> tys.Type:
-        return tys.Opaque(
-            extension="Collections",
-            id="List",
-            args=[tys.TypeTypeArg(ty=self.element_type.to_hugr())],
-            bound=self.hugr_bound(),
-        )
-
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
-        return transformer.transform(self) or ListType(
-            self.element_type.transform(transformer)
-        )
-
-
-@dataclass(frozen=True)
-class LinstType(GuppyType):
-    element_type: GuppyType
-
-    name: ClassVar[Literal["linst"]] = "linst"
-
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        from guppylang.error import GuppyError
-
-        if len(args) == 0:
-            raise GuppyError("Missing type parameter for generic type `linst`", node)
-        if len(args) > 1:
-            raise GuppyError("Too many type arguments for generic type `linst`", node)
-        return LinstType(args[0])
+    For example, many builtin types like `int`, `float`, `list` etc. are directly backed
+    by a Hugr extension.
+    """
 
-    def __str__(self) -> str:
-        return f"linst[{self.element_type}]"
+    defn: "OpaqueTypeDef"
 
     @property
-    def linear(self) -> bool:
-        return self.element_type.linear
+    def intrinsically_linear(self) -> bool:
+        """Whether this type is linear, independent of the arguments."""
+        return self.defn.always_linear
 
     @property
-    def type_args(self) -> Iterator[GuppyType]:
-        return iter((self.element_type,))
+    def hugr_bound(self) -> tys.TypeBound:
+        """The Hugr bound of this type, i.e. `Any`, `Copyable`, or `Equatable`."""
+        if self.defn.bound is not None:
+            return self.defn.bound
+        return super().hugr_bound
 
     def to_hugr(self) -> tys.Type:
-        return tys.Opaque(
-            extension="Collections",
-            id="List",
-            args=[tys.TypeTypeArg(ty=self.element_type.to_hugr())],
-            bound=self.hugr_bound(),
-        )
+        """Computes the Hugr representation of the type."""
+        return self.defn.to_hugr(self.args)
 
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
-        return transformer.transform(self) or LinstType(
-            self.element_type.transform(transformer)
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
+        return transformer.transform(self) or OpaqueType(
+            [arg.transform(transformer) for arg in self.args], self.defn
         )
 
 
-@dataclass(frozen=True)
-class NoneType(GuppyType):
-    name: ClassVar[Literal["None"]] = "None"
-    linear: bool = False
+# We define the `Type` type as a union of all `TypeBase` subclasses defined above. This
+# models an algebraic data type and enables exhaustiveness checking in pattern matches
+# etc.
+# Note that this might become obsolete in case the `@sealed` decorator is added:
+#  * https://peps.python.org/pep-0622/#sealed-classes-as-algebraic-data-types
+#  * https://github.com/johnthagen/sealed-typing-pep
+ParametrizedType: TypeAlias = FunctionType | TupleType | SumType | OpaqueType
+Type: TypeAlias = BoundTypeVar | ExistentialTypeVar | NoneType | ParametrizedType
 
-    # Flag to avoid turning the type into a row when calling `type_to_row()`. This is
-    # used to make sure that type vars instantiated to Nones are not broken up into
-    # empty rows when generating a Hugr
-    preserve: bool = field(default=False, compare=False)
+TypeRow: TypeAlias = Sequence[Type]
 
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        if len(args) > 0:
-            from guppylang.error import GuppyError
 
-            raise GuppyError("Type `None` is not generic", node)
+def row_to_type(row: TypeRow) -> Type:
+    """Turns a row of types into a single type by packing into a tuple."""
+    if len(row) == 0:
         return NoneType()
+    elif len(row) == 1:
+        return row[0]
+    else:
+        return TupleType(row)
 
-    @property
-    def type_args(self) -> Iterator[GuppyType]:
-        return iter(())
-
-    def substitute(self, s: Subst) -> GuppyType:
-        return self
-
-    def __str__(self) -> str:
-        return "None"
-
-    def to_hugr(self) -> tys.Type:
-        return tys.TupleType(inner=[])
-
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
-        return transformer.transform(self) or self
-
-
-@dataclass(frozen=True)
-class BoolType(SumType):
-    """The type of booleans."""
-
-    linear: bool = False
-    name: ClassVar[Literal["bool"]] = "bool"
-
-    def __init__(self) -> None:
-        # Hugr bools are encoded as Sum((), ())
-        super().__init__([TupleType([]), TupleType([])])
-
-    @staticmethod
-    def build(*args: GuppyType, node: AstNode | None = None) -> GuppyType:
-        if len(args) > 0:
-            from guppylang.error import GuppyError
-
-            raise GuppyError("Type `bool` is not generic", node)
-        return BoolType()
-
-    def __str__(self) -> str:
-        return "bool"
-
-    def transform(self, transformer: "TypeTransformer") -> GuppyType:
-        return transformer.transform(self) or self
-
-
-class TypeTransformer(ABC):
-    """Abstract base class for a type visitor that transforms types."""
-
-    @abstractmethod
-    def transform(self, ty: GuppyType) -> GuppyType | None:
-        """This method is called for each visited type.
-
-        Return a transformed type or `None` to continue the recursive visit.
-        """
-
-
-class Substituter(TypeTransformer):
-    """Type transformer that substitutes free type variables."""
-
-    subst: Subst
-
-    def __init__(self, subst: Subst) -> None:
-        self.subst = subst
-
-    def transform(self, ty: GuppyType) -> GuppyType | None:
-        if isinstance(ty, ExistentialTypeVar):
-            return self.subst.get(ty, None)
-        return None
-
-
-class Instantiator(TypeTransformer):
-    """Type transformer that instantiates bound type variables."""
-
-    tys: Sequence[GuppyType]
-
-    def __init__(self, tys: Sequence[GuppyType]) -> None:
-        self.tys = tys
-
-    def transform(self, ty: GuppyType) -> GuppyType | None:
-        if isinstance(ty, BoundTypeVar):
-            # Instantiate if type for the index is available
-            if ty.idx < len(self.tys):
-                return self.tys[ty.idx]
 
-            # Otherwise, lower the de Bruijn index
-            return BoundTypeVar(ty.idx - len(self.tys), ty.display_name, ty.linear)
-        return None
+def type_to_row(ty: Type) -> TypeRow:
+    """Turns a type into a row of types by unpacking top-level tuples."""
+    if isinstance(ty, NoneType) and not ty.preserve:
+        return []
+    if isinstance(ty, TupleType) and not ty.preserve:
+        return ty.element_types
+    return [ty]
 
 
-def unify(s: GuppyType, t: GuppyType, subst: Subst | None) -> Subst | None:
+def unify(s: Type, t: Type, subst: "Subst | None") -> "Subst | None":
     """Computes a most general unifier for two types.
 
     Return a substitutions `subst` such that `s[subst] == t[subst]` or `None` if this
     not possible.
     """
     if subst is None:
         return None
-    if s == t:
-        return subst
-    if isinstance(s, ExistentialTypeVar):
-        return _unify_var(s, t, subst)
-    if isinstance(t, ExistentialTypeVar):
-        return _unify_var(t, s, subst)
-    if type(s) == type(t):
-        sargs, targs = list(s.type_args), list(t.type_args)
-        if len(sargs) == len(targs):
-            for sa, ta in zip(sargs, targs):
-                subst = unify(sa, ta, subst)
+    match s, t:
+        case ExistentialTypeVar(id=s_id), ExistentialTypeVar(id=t_id) if s_id == t_id:
+            return subst
+        case ExistentialTypeVar() as s, t:
+            return _unify_var(s, t, subst)
+        case s, ExistentialTypeVar() as t:
+            return _unify_var(t, s, subst)
+        case BoundTypeVar(idx=s_idx), BoundTypeVar(idx=t_idx) if s_idx == t_idx:
             return subst
-    return None
+        case NoneType(), NoneType():
+            return subst
+        case FunctionType() as s, FunctionType() as t if s.params == t.params:
+            return _unify_args(s, t, subst)
+        case TupleType() as s, TupleType() as t:
+            return _unify_args(s, t, subst)
+        case SumType() as s, SumType() as t:
+            return _unify_args(s, t, subst)
+        case OpaqueType() as s, OpaqueType() as t if s.defn == t.defn:
+            return _unify_args(s, t, subst)
+        case _:
+            return None
 
 
-def _unify_var(var: ExistentialTypeVar, t: GuppyType, subst: Subst) -> Subst | None:
+def _unify_var(var: ExistentialTypeVar, t: Type, subst: "Subst") -> "Subst | None":
     """Helper function for unification of type variables."""
     if var in subst:
         return unify(subst[var], t, subst)
     if isinstance(t, ExistentialTypeVar) and t in subst:
         return unify(var, subst[t], subst)
     if var in t.unsolved_vars:
         return None
     return {var: t, **subst}
 
 
-def type_from_ast(
-    node: AstNode,
-    globals: "Globals",
-    type_var_mapping: dict[str, BoundTypeVar] | None = None,
-) -> GuppyType:
-    """Turns an AST expression into a Guppy type."""
-    from guppylang.error import GuppyError
-
-    if isinstance(node, ast.Name):
-        x = node.id
-        if x in globals.types:
-            return globals.types[x].build(node=node)
-        if x in globals.type_vars:
-            if type_var_mapping is None:
-                raise GuppyError(
-                    "Free type variable. Only function types can be generic", node
-                )
-            var_decl = globals.type_vars[x]
-            if var_decl.name not in type_var_mapping:
-                type_var_mapping[var_decl.name] = BoundTypeVar(
-                    len(type_var_mapping), var_decl.name, var_decl.linear
-                )
-            return type_var_mapping[var_decl.name]
-        raise GuppyError("Unknown type", node)
-
-    if isinstance(node, ast.Constant):
-        v = node.value
-        if v is None:
-            return NoneType()
-        if isinstance(v, str):
-            try:
-                [stmt] = ast.parse(v).body
-                if not isinstance(stmt, ast.Expr):
-                    raise GuppyError("Invalid Guppy type", node)
-                return type_from_ast(stmt.value, globals, type_var_mapping)
-            except (SyntaxError, ValueError):
-                raise GuppyError("Invalid Guppy type", node) from None
-        raise GuppyError(f"Constant `{v}` is not a valid type", node)
-
-    if isinstance(node, ast.Tuple):
-        return TupleType(
-            [type_from_ast(el, globals, type_var_mapping) for el in node.elts]
-        )
-
-    if (
-        isinstance(node, ast.Subscript)
-        and isinstance(node.value, ast.Name)
-        and node.value.id == "Callable"
-        and isinstance(node.slice, ast.Tuple)
-        and len(node.slice.elts) == 2
-    ):
-        # TODO: Do we want to allow polymorphic Callable types?
-        [func_args, ret] = node.slice.elts
-        if isinstance(func_args, ast.List):
-            return FunctionType(
-                [type_from_ast(a, globals, type_var_mapping) for a in func_args.elts],
-                type_from_ast(ret, globals, type_var_mapping),
-            )
-
-    if isinstance(node, ast.Subscript) and isinstance(node.value, ast.Name):
-        x = node.value.id
-        if x in globals.types:
-            args = (
-                node.slice.elts if isinstance(node.slice, ast.Tuple) else [node.slice]
-            )
-            return globals.types[x].build(
-                *(type_from_ast(a, globals, type_var_mapping) for a in args), node=node
-            )
-
-    raise GuppyError("Not a valid Guppy type", node)
-
-
-def type_row_from_ast(node: ast.expr, globals: "Globals") -> Sequence[GuppyType]:
-    """Turns an AST expression into a Guppy type row.
-
-    This is needed to interpret the return type annotation of functions.
-    """
-    # The return type `-> None` is represented in the ast as `ast.Constant(value=None)`
-    if isinstance(node, ast.Constant) and node.value is None:
-        return []
-    ty = type_from_ast(node, globals)
-    if isinstance(ty, TupleType):
-        return ty.element_types
-    else:
-        return [ty]
-
-
-def row_to_type(row: Sequence[GuppyType]) -> GuppyType:
-    """Turns a row of types into a single type by packing into a tuple."""
-    if len(row) == 0:
-        return NoneType()
-    elif len(row) == 1:
-        return row[0]
-    else:
-        return TupleType(row)
-
-
-def type_to_row(ty: GuppyType) -> Sequence[GuppyType]:
-    """Turns a type into a row of types by unpacking top-level tuples."""
-    if isinstance(ty, NoneType) and not ty.preserve:
-        return []
-    if isinstance(ty, TupleType) and not ty.preserve:
-        return ty.element_types
-    return [ty]
+def _unify_args(
+    s: ParametrizedType, t: ParametrizedType, subst: "Subst"
+) -> "Subst | None":
+    """Helper function for unification of type arguments of parametrised types."""
+    if len(s.args) != len(t.args):
+        return None
+    for sa, ta in zip(s.args, t.args, strict=True):
+        match sa, ta:
+            case TypeArg(ty=sa_ty), TypeArg(ty=ta_ty):
+                res = unify(sa_ty, ta_ty, subst)
+                if res is None:
+                    return None
+                subst = res
+            case ConstArg(), ConstArg():
+                raise NotImplementedError
+            case _:
+                return None
+    return subst
```

### Comparing `guppylang-0.1.0/guppylang/hugr/hugr.py` & `guppylang-0.2.0/guppylang/hugr/hugr.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from dataclasses import dataclass, field
 from typing import Any, Optional
 
 import networkx as nx  # type: ignore[import-untyped]
 
 import guppylang.hugr.ops as ops
 import guppylang.hugr.raw as raw
-from guppylang.gtypes import (
+from guppylang.hugr import val
+from guppylang.tys.subst import Inst
+from guppylang.tys.ty import (
     FunctionType,
-    GuppyType,
-    Inst,
     SumType,
     TupleType,
+    Type,
     row_to_type,
     type_to_row,
 )
-from guppylang.hugr import tys, val
 
 NodeIdx = int
 PortOffset = int
 
 
 @dataclass(frozen=True)
 class Port(ABC):
@@ -40,23 +40,23 @@
     """Base class for a port that outgoing wires come from."""
 
 
 @dataclass(frozen=True)
 class InPortV(InPort):
     """A typed value input port."""
 
-    ty: GuppyType
+    ty: Type
     offset: PortOffset
 
 
 @dataclass(frozen=True)
 class OutPortV(OutPort):
     """A typed value output port."""
 
-    ty: GuppyType
+    ty: Type
     offset: PortOffset
 
 
 @dataclass(frozen=True)
 class InPortCF(InPort):
     """A control-flow input port."""
 
@@ -66,15 +66,15 @@
 
 class OutPortCF(OutPort):
     """A control-flow output port."""
 
 
 Edge = tuple[OutPort, InPort]
 
-TypeList = list[GuppyType]
+TypeList = list[Type]
 
 
 @dataclass
 class Node(ABC):
     """Base class for a node in the graph.
 
     Has a number of input and output ports and an associated op type.
@@ -134,21 +134,21 @@
         return len(self.in_port_types)
 
     @property
     def num_out_ports(self) -> int:
         """The number of output ports on this node."""
         return len(self.out_port_types)
 
-    def add_in_port(self, ty: GuppyType) -> InPortV:
+    def add_in_port(self, ty: Type) -> InPortV:
         """Adds an input port at the end of the node and returns the port."""
         p = InPortV(self, self.num_in_ports, ty)
         self.in_port_types.append(ty)
         return p
 
-    def add_out_port(self, ty: GuppyType) -> OutPortV:
+    def add_out_port(self, ty: Type) -> OutPortV:
         """Adds an output port at the end of the node and returns the port."""
         p = OutPortV(self, self.num_out_ports, ty)
         self.out_port_types.append(ty)
         return p
 
     def in_port(self, offset: PortOffset | None) -> InPortV:
         """Returns the input port at the given offset."""
@@ -350,15 +350,15 @@
 
     def set_root_name(self, name: str) -> VNode:
         """Sets the name of the root node."""
         self.root.meta_data["name"] = name
         return self.root
 
     def add_constant(
-        self, value: val.Value, ty: GuppyType, parent: Node | None = None
+        self, value: val.Value, ty: Type, parent: Node | None = None
     ) -> VNode:
         """Adds a constant node holding a given value to the graph."""
         return self.add_node(
             ops.Const(value=value, typ=ty.to_hugr()), [], [ty], parent, None
         )
 
     def add_input(
@@ -368,15 +368,15 @@
         parent = parent or self._default_parent
         node = self.add_node(ops.Input(), [], output_tys, parent)
         if isinstance(parent, DFContainingNode):
             parent.input_child = node
         return node
 
     def add_input_with_ports(
-        self, output_tys: Sequence[GuppyType], parent: Node | None = None
+        self, output_tys: Sequence[Type], parent: Node | None = None
     ) -> tuple[VNode, list[OutPortV]]:
         """Adds an `Input` node to the graph."""
         node = self.add_input(None, parent)
         ports = [node.add_out_port(ty) for ty in output_tys]
         return node, ports
 
     def add_output(
@@ -491,60 +491,60 @@
         self, def_port: OutPortV, args: list[OutPortV], parent: Node | None = None
     ) -> VNode:
         """Adds a `Call` node to the graph."""
         assert isinstance(def_port.ty, FunctionType)
         return self.add_node(
             ops.Call(),
             None,
-            list(type_to_row(def_port.ty.returns)),
+            list(type_to_row(def_port.ty.output)),
             parent,
             [*args, def_port],
         )
 
     def add_indirect_call(
         self, fun_port: OutPortV, args: list[OutPortV], parent: Node | None = None
     ) -> VNode:
         """Adds an `IndirectCall` node to the graph."""
         assert isinstance(fun_port.ty, FunctionType)
         return self.add_node(
             ops.CallIndirect(),
             None,
-            list(type_to_row(fun_port.ty.returns)),
+            list(type_to_row(fun_port.ty.output)),
             parent,
             [fun_port, *args],
         )
 
     def add_partial(
-        self, def_port: OutPortV, args: list[OutPortV], parent: Node | None = None
+        self, def_port: OutPortV, inputs: list[OutPortV], parent: Node | None = None
     ) -> VNode:
         """Adds a `Partial` evaluation node to the graph."""
         assert isinstance(def_port.ty, FunctionType)
-        assert len(def_port.ty.args) >= len(args)
-        assert [p.ty for p in args] == def_port.ty.args[: len(args)]
+        assert len(def_port.ty.inputs) >= len(inputs)
+        assert [p.ty for p in inputs] == def_port.ty.inputs[: len(inputs)]
         new_ty = FunctionType(
-            def_port.ty.args[len(args) :],
-            def_port.ty.returns,
-            def_port.ty.arg_names[len(args) :]
-            if def_port.ty.arg_names is not None
+            def_port.ty.inputs[len(inputs) :],
+            def_port.ty.output,
+            def_port.ty.input_names[len(inputs) :]
+            if def_port.ty.input_names is not None
             else None,
         )
         return self.add_node(
-            ops.DummyOp(name="partial"), None, [new_ty], parent, [*args, def_port]
+            ops.DummyOp(name="partial"), None, [new_ty], parent, [*inputs, def_port]
         )
 
     def add_type_apply(
         self, func_port: OutPortV, args: Inst, parent: Node | None = None
     ) -> VNode:
         """Adds a `TypeApply` node to the graph."""
         assert isinstance(func_port.ty, FunctionType)
-        assert len(func_port.ty.quantified) == len(args)
+        assert len(func_port.ty.params) == len(args)
         result_ty = func_port.ty.instantiate(args)
         ta = ops.TypeApplication(
             input=func_port.ty.to_hugr(),
-            args=[tys.TypeTypeArg(ty=ty.to_hugr()) for ty in args],
+            args=[arg.to_hugr() for arg in args],
             output=result_ty.to_hugr(),
         )
         return self.add_node(
             ops.TypeApply(ta=ta),
             inputs=[func_port],
             output_types=[result_ty],
             parent=parent,
```

### Comparing `guppylang-0.1.0/guppylang/hugr/ops.py` & `guppylang-0.2.0/guppylang/hugr/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,15 +418,14 @@
 
 OpType = TypeAliasType(
     "OpType",
     Annotated[
         (
             Module
             | Case
-            | Module
             | FuncDefn
             | FuncDecl
             | Const
             | DummyOp
             | DataflowBlock
             | ExitBlock
             | Conditional
```

### Comparing `guppylang-0.1.0/guppylang/hugr/raw.py` & `guppylang-0.2.0/guppylang/hugr/raw.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.1.0/guppylang/hugr/tys.py` & `guppylang-0.2.0/guppylang/hugr/tys.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.1.0/guppylang/hugr/val.py` & `guppylang-0.2.0/guppylang/hugr/val.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.1.0/guppylang/hugr/visualise.py` & `guppylang-0.2.0/guppylang/hugr/visualise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Visualise HUGR using graphviz."""
+
 import ast
 from collections.abc import Iterable
 from typing import TYPE_CHECKING
 
 import graphviz as gv  # type: ignore[import-untyped]
 
 from guppylang.cfg.analysis import (
```

### Comparing `guppylang-0.1.0/guppylang/module.py` & `guppylang-0.2.0/guppylang/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import sys
 import textwrap
 from collections.abc import Callable
 from types import ModuleType
 from typing import Any, Union
 
 from guppylang.ast_util import AstNode, annotate_location
-from guppylang.checker.core import Globals, PyScope, TypeVarDecl, qualified_name
+from guppylang.checker.core import Globals, PyScope, qualified_name
 from guppylang.checker.func_checker import DefinedFunction, check_global_func_def
 from guppylang.compiler.core import CompiledGlobals
 from guppylang.compiler.func_compiler import (
     CompiledFunctionDef,
     compile_global_func_def,
 )
 from guppylang.custom import CustomFunction
 from guppylang.declared import DeclaredFunction
 from guppylang.error import GuppyError, pretty_errors
-from guppylang.gtypes import GuppyType
 from guppylang.hugr.hugr import Hugr
+from guppylang.tys.definition import TypeDef
+from guppylang.tys.param import TypeParam
 
 PyFunc = Callable[..., Any]
 PyFuncDefOrDecl = tuple[bool, PyFunc]
 
 
 class GuppyModule:
     """A Guppy module that may contain function and type definitions."""
@@ -88,82 +89,80 @@
             self._imported_globals |= m._globals
             self._imported_compiled_globals |= m._compiled_globals
         else:
             for val in m.__dict__.values():
                 if isinstance(val, GuppyModule):
                     self.load(val)
 
-    def register_func_def(
-        self, f: PyFunc, instance: type[GuppyType] | None = None
-    ) -> None:
+    def register_func_def(self, f: PyFunc, instance: TypeDef | None = None) -> None:
         """Registers a Python function definition as belonging to this Guppy module."""
         self._check_not_yet_compiled()
         func_ast = parse_py_func(f)
         if self._instance_func_buffer is not None:
             self._instance_func_buffer[func_ast.name] = (True, f)
         else:
             name = (
                 qualified_name(instance, func_ast.name) if instance else func_ast.name
             )
             self._check_name_available(name, func_ast)
             self._func_defs[name] = func_ast, get_py_scope(f)
 
-    def register_func_decl(
-        self, f: PyFunc, instance: type[GuppyType] | None = None
-    ) -> None:
+    def register_func_decl(self, f: PyFunc, instance: TypeDef | None = None) -> None:
         """Registers a Python function declaration as belonging to this Guppy module."""
         self._check_not_yet_compiled()
         func_ast = parse_py_func(f)
         if self._instance_func_buffer is not None:
             self._instance_func_buffer[func_ast.name] = (False, f)
         else:
             name = (
                 qualified_name(instance, func_ast.name) if instance else func_ast.name
             )
             self._check_name_available(name, func_ast)
             self._func_decls[name] = func_ast
 
     def register_custom_func(
-        self, func: CustomFunction, instance: type[GuppyType] | None = None
+        self, func: CustomFunction, instance: TypeDef | None = None
     ) -> None:
         """Registers a custom function as belonging to this Guppy module."""
         self._check_not_yet_compiled()
         if self._instance_func_buffer is not None:
             self._instance_func_buffer[func.name] = func
         else:
             if instance:
                 func.name = qualified_name(instance, func.name)
             self._check_name_available(func.name, func.defined_at)
             self._custom_funcs[func.name] = func
 
-    def register_type(self, name: str, ty: type[GuppyType]) -> None:
+    def register_type(self, name: str, defn: TypeDef) -> None:
         """Registers an existing Guppy type as belonging to this Guppy module."""
         self._check_not_yet_compiled()
         self._check_type_name_available(name, None)
-        self._globals.types[name] = ty
+        self._globals.type_defs[name] = defn
 
     def register_type_var(self, name: str, linear: bool) -> None:
         """Registers a new type variable"""
         self._check_not_yet_compiled()
         self._check_type_name_available(name, None)
-        self._globals.type_vars[name] = TypeVarDecl(name, linear)
+        self._globals.param_vars[name] = TypeParam(
+            len(self._globals.param_vars), name, linear
+        )
 
-    def _register_buffered_instance_funcs(self, instance: type[GuppyType]) -> None:
+    def _register_buffered_instance_funcs(self, defn: TypeDef) -> None:
         assert self._instance_func_buffer is not None
         buffer = self._instance_func_buffer
         self._instance_func_buffer = None
         for f in buffer.values():
             if isinstance(f, CustomFunction):
-                self.register_custom_func(f, instance)
+                self.register_custom_func(f, defn)
             else:
                 is_def, pyfunc = f
                 if is_def:
-                    self.register_func_def(pyfunc, instance)
+                    self.register_func_def(pyfunc, defn)
                 else:
-                    self.register_func_decl(pyfunc, instance)
+                    self.register_func_decl(pyfunc, defn)
 
     @property
     def compiled(self) -> bool:
         return self._compiled
 
     @pretty_errors
     def compile(self) -> Hugr | None:
@@ -228,35 +227,35 @@
 
     def contains_function(self, name: str) -> bool:
         """Returns 'True' if the module contains a function with the given name."""
         return name in self._func_defs or name in self._custom_funcs
 
     def contains_type(self, name: str) -> bool:
         """Returns 'True' if the module contains a type with the given name."""
-        return name in self._globals.types or name in self._globals.type_vars
+        return name in self._globals.type_defs or name in self._globals.param_vars
 
     def _check_not_yet_compiled(self) -> None:
         if self._compiled:
             raise GuppyError(f"The module `{self.name}` has already been compiled")
 
     def _check_name_available(self, name: str, node: AstNode | None) -> None:
         if self.contains_function(name):
             raise GuppyError(
                 f"Module `{self.name}` already contains a function named `{name}`",
                 node,
             )
 
     def _check_type_name_available(self, name: str, node: AstNode | None) -> None:
-        if name in self._globals.types:
+        if name in self._globals.type_defs:
             raise GuppyError(
                 f"Module `{self.name}` already contains a type `{name}`",
                 node,
             )
 
-        if name in self._globals.type_vars:
+        if name in self._globals.param_vars:
             raise GuppyError(
                 f"Module `{self.name}` already contains a type variable `{name}`",
                 node,
             )
 
 
 def parse_py_func(f: PyFunc) -> ast.FunctionDef:
```

### Comparing `guppylang-0.1.0/guppylang/nodes.py` & `guppylang-0.2.0/guppylang/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Custom AST nodes used by Guppy"""
 
 import ast
-from collections.abc import Mapping, Sequence
+from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any
 
-from guppylang.gtypes import FunctionType, GuppyType, Inst
+from guppylang.tys.subst import Inst
+from guppylang.tys.ty import FunctionType
 
 if TYPE_CHECKING:
     from guppylang.cfg.cfg import CFG
     from guppylang.checker.cfg_checker import CheckedCFG
     from guppylang.checker.core import CallableVariable, Variable
 
 
@@ -48,19 +49,19 @@
         "args",
         "type_args",
     )
 
 
 class TypeApply(ast.expr):
     value: ast.expr
-    tys: Sequence[GuppyType]
+    inst: Inst
 
     _fields = (
         "value",
-        "tys",
+        "inst",
     )
 
 
 class MakeIter(ast.expr):
     """Creates an iterator using the `__iter__` magic method.
 
     This node is inserted in `for` loops and list comprehensions.
```

### Comparing `guppylang-0.1.0/guppylang/prelude/_internal.py` & `guppylang-0.2.0/guppylang/prelude/_internal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import ast
-from typing import Literal
+from typing import Any, Literal
 
 from pydantic import BaseModel
 
 from guppylang.ast_util import AstNode, get_type, with_loc, with_type
 from guppylang.checker.core import CallableVariable, Context
 from guppylang.checker.expr_checker import ExprSynthesizer, check_num_args
 from guppylang.custom import (
     CustomCallChecker,
     CustomCallCompiler,
     CustomFunction,
     DefaultCallChecker,
 )
 from guppylang.error import GuppyError, GuppyTypeError
-from guppylang.gtypes import BoolType, FunctionType, GuppyType, Subst, unify
 from guppylang.hugr import ops, tys, val
 from guppylang.hugr.hugr import OutPortV
 from guppylang.nodes import GlobalCall
+from guppylang.tys.definition import bool_type
+from guppylang.tys.subst import Subst
+from guppylang.tys.ty import FunctionType, OpaqueType, Type, unify
 
 INT_WIDTH = 6  # 2^6 = 64 bit
 
 
 hugr_int_type = tys.Opaque(
     extension="arithmetic.int.types",
     id="int",
@@ -48,14 +50,21 @@
 class ConstF64(BaseModel):
     """Hugr representation of floats in the arithmetic extension."""
 
     c: Literal["ConstF64"] = "ConstF64"
     value: float
 
 
+class ListValue(BaseModel):
+    """Hugr representation of floats in the arithmetic extension."""
+
+    c: Literal["ListValue"] = "ListValue"
+    value: tuple[list[Any], tys.Type]
+
+
 def bool_value(b: bool) -> val.Value:
     """Returns the Hugr representation of a boolean value."""
     return val.Sum(tag=int(b), value=val.Tuple(vs=[]))
 
 
 def int_value(i: int) -> val.Value:
     """Returns the Hugr representation of an integer value."""
@@ -63,14 +72,19 @@
 
 
 def float_value(f: float) -> val.Value:
     """Returns the Hugr representation of a float value."""
     return val.ExtensionVal(c=(ConstF64(value=f),))
 
 
+def list_value(v: list[val.Value], ty: tys.Type) -> val.Value:
+    """Returns the Hugr representation of a list value."""
+    return val.ExtensionVal(c=(ListValue(value=(v, ty)),))
+
+
 def logic_op(op_name: str, args: list[tys.TypeArg] | None = None) -> ops.OpType:
     """Utility method to create Hugr logic ops."""
     return ops.CustomOp(extension="logic", op_name=op_name, args=args or [])
 
 
 def int_op(
     op_name: str, ext: str = "arithmetic.int", num_params: int = 1
@@ -87,25 +101,30 @@
     """Utility method to create Hugr integer arithmetic ops."""
     return ops.CustomOp(extension=ext, op_name=op_name, args=[])
 
 
 class CoercingChecker(DefaultCallChecker):
     """Function call type checker that automatically coerces arguments to float."""
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         from .builtins import Int
 
         for i in range(len(args)):
             args[i], ty = ExprSynthesizer(self.ctx).synthesize(args[i])
-            if isinstance(ty, self.ctx.globals.types["int"]):
+            if (
+                isinstance(ty, OpaqueType)
+                and ty.defn == self.ctx.globals.type_defs["int"]
+            ):
                 call = with_loc(
                     self.node,
                     GlobalCall(func=Int.__float__, args=[args[i]], type_args=[]),
                 )
-                args[i] = with_type(self.ctx.globals.types["float"].build(), call)
+                args[i] = with_type(
+                    self.ctx.globals.type_defs["float"].check_instantiate([]), call
+                )
         return super().synthesize(args)
 
 
 class ReversingChecker(CustomCallChecker):
     """Call checker that reverses the arguments after checking."""
 
     base_checker: CustomCallChecker
@@ -113,21 +132,21 @@
     def __init__(self, base_checker: CustomCallChecker | None = None):
         self.base_checker = base_checker or DefaultCallChecker()
 
     def _setup(self, ctx: Context, node: AstNode, func: CustomFunction) -> None:
         super()._setup(ctx, node, func)
         self.base_checker._setup(ctx, node, func)
 
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         expr, subst = self.base_checker.check(args, ty)
         if isinstance(expr, GlobalCall):
             expr.args = list(reversed(args))
         return expr, subst
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         expr, ty = self.base_checker.synthesize(args)
         if isinstance(expr, GlobalCall):
             expr.args = list(reversed(args))
         return expr, ty
 
 
 class FailingChecker(CustomCallChecker):
@@ -135,33 +154,33 @@
 
     Gives the uses a nicer error message when they try to use an unsupported feature.
     """
 
     def __init__(self, msg: str) -> None:
         self.msg = msg
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         raise GuppyError(self.msg, self.node)
 
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         raise GuppyError(self.msg, self.node)
 
 
 class UnsupportedChecker(CustomCallChecker):
     """Call checker for Python builtin functions that are not available in Guppy.
 
     Gives the uses a nicer error message when they try to use an unsupported feature.
     """
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         raise GuppyError(
             f"Builtin method `{self.func.name}` is not supported by Guppy", self.node
         )
 
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         raise GuppyError(
             f"Builtin method `{self.func.name}` is not supported by Guppy", self.node
         )
 
 
 class DunderChecker(CustomCallChecker):
     """Call checker for builtin functions that call out to dunder instance methods"""
@@ -185,40 +204,40 @@
             raise GuppyTypeError(
                 f"Builtin function `{self.func.name}` is not defined for argument of "
                 f"type `{ty}`",
                 self.node.args[0] if isinstance(self.node, ast.Call) else self.node,
             )
         return [fst, *rest], func
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         args, func = self._get_func(args)
         return func.synthesize_call(args, self.node, self.ctx)
 
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         args, func = self._get_func(args)
         return func.check_call(args, ty, self.node, self.ctx)
 
 
 class CallableChecker(CustomCallChecker):
     """Call checker for the builtin `callable` function"""
 
-    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, GuppyType]:
+    def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         check_num_args(1, len(args), self.node)
         [arg] = args
         arg, ty = ExprSynthesizer(self.ctx).synthesize(arg)
         is_callable = (
             isinstance(ty, FunctionType)
             or self.ctx.globals.get_instance_func(ty, "__call__") is not None
         )
         const = with_loc(self.node, ast.Constant(value=is_callable))
-        return const, BoolType()
+        return const, bool_type()
 
-    def check(self, args: list[ast.expr], ty: GuppyType) -> tuple[ast.expr, Subst]:
+    def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         args, _ = self.synthesize(args)
-        subst = unify(ty, BoolType(), {})
+        subst = unify(ty, bool_type(), {})
         if subst is None:
             raise GuppyTypeError(
                 f"Expected expression of type `{ty}`, got `bool`", self.node
             )
         return args, subst
 
 
@@ -320,8 +339,8 @@
         from .quantum import quantum_op
 
         [qubit] = args
         measure = self.graph.add_node(quantum_op("Measure"), inputs=args)
         self.graph.add_node(
             quantum_op("QFree"), inputs=[measure.add_out_port(qubit.ty)]
         )
-        return [measure.add_out_port(BoolType())]
+        return [measure.add_out_port(bool_type())]
```

### Comparing `guppylang-0.1.0/guppylang/prelude/builtins.py` & `guppylang-0.2.0/guppylang/prelude/builtins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Guppy module for builtin types and operations."""
 
 # mypy: disable-error-code="empty-body, misc, override, valid-type, no-untyped-def"
 
 from guppylang.custom import DefaultCallChecker, NoopCompiler
 from guppylang.decorator import guppy
-from guppylang.gtypes import BoolType, LinstType, ListType
 from guppylang.hugr import ops, tys
 from guppylang.module import GuppyModule
 from guppylang.prelude._internal import (
     CallableChecker,
     CoercingChecker,
     DunderChecker,
     FailingChecker,
@@ -21,865 +20,682 @@
     UnsupportedChecker,
     float_op,
     hugr_float_type,
     hugr_int_type,
     int_op,
     logic_op,
 )
+from guppylang.tys.definition import bool_type_def, linst_type_def, list_type_def
 
 builtins = GuppyModule("builtins", import_builtins=False)
 
 T = guppy.type_var(builtins, "T")
 L = guppy.type_var(builtins, "L", linear=True)
 
 
-@guppy.extend_type(builtins, BoolType)
+@guppy.extend_type(builtins, bool_type_def)
 class Bool:
     @guppy.hugr_op(builtins, logic_op("And", [tys.BoundedNatArg(n=2)]))
-    def __and__(self: bool, other: bool) -> bool:
-        ...
+    def __and__(self: bool, other: bool) -> bool: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __bool__(self: bool) -> bool:
-        ...
+    def __bool__(self: bool) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("ifrombool"))
-    def __int__(self: bool) -> int:
-        ...
+    def __int__(self: bool) -> int: ...
 
     @guppy.hugr_op(builtins, logic_op("Or", [tys.BoundedNatArg(n=2)]))
-    def __or__(self: bool, other: bool) -> bool:
-        ...
+    def __or__(self: bool, other: bool) -> bool: ...
 
 
 @guppy.type(builtins, hugr_int_type, name="int")
 class Int:
     @guppy.hugr_op(builtins, int_op("iabs"))  # TODO: Maybe wrong? (signed vs unsigned!)
-    def __abs__(self: int) -> int:
-        ...
+    def __abs__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("iadd"))
-    def __add__(self: int, other: int) -> int:
-        ...
+    def __add__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("iand"))
-    def __and__(self: int, other: int) -> int:
-        ...
+    def __and__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("itobool"))
-    def __bool__(self: int) -> bool:
-        ...
+    def __bool__(self: int) -> bool: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __ceil__(self: int) -> int:
-        ...
+    def __ceil__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("idivmod_s", num_params=2))
-    def __divmod__(self: int, other: int) -> tuple[int, int]:
-        ...
+    def __divmod__(self: int, other: int) -> tuple[int, int]: ...
 
     @guppy.hugr_op(builtins, int_op("ieq"))
-    def __eq__(self: int, other: int) -> bool:
-        ...
+    def __eq__(self: int, other: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("convert_s", "arithmetic.conversions"))
-    def __float__(self: int) -> float:
-        ...
+    def __float__(self: int) -> float: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __floor__(self: int) -> int:
-        ...
+    def __floor__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("idiv_s", num_params=2))
-    def __floordiv__(self: int, other: int) -> int:
-        ...
+    def __floordiv__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ige_s"))
-    def __ge__(self: int, other: int) -> bool:
-        ...
+    def __ge__(self: int, other: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("igt_s"))
-    def __gt__(self: int, other: int) -> bool:
-        ...
+    def __gt__(self: int, other: int) -> bool: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __int__(self: int) -> int:
-        ...
+    def __int__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("inot"))
-    def __invert__(self: int) -> bool:
-        ...
+    def __invert__(self: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("ile_s"))
-    def __le__(self: int, other: int) -> bool:
-        ...
+    def __le__(self: int, other: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("ishl", num_params=2))  # TODO: RHS is unsigned
-    def __lshift__(self: int, other: int) -> int:
-        ...
+    def __lshift__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ilt_s"))
-    def __lt__(self: int, other: int) -> bool:
-        ...
+    def __lt__(self: int, other: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("imod_s", num_params=2))
-    def __mod__(self: int, other: int) -> int:
-        ...
+    def __mod__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("imul"))
-    def __mul__(self: int, other: int) -> int:
-        ...
+    def __mul__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ine"))
-    def __ne__(self: int, other: int) -> bool:
-        ...
+    def __ne__(self: int, other: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("ineg"))
-    def __neg__(self: int) -> int:
-        ...
+    def __neg__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ior"))
-    def __or__(self: int, other: int) -> int:
-        ...
+    def __or__(self: int, other: int) -> int: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __pos__(self: int) -> int:
-        ...
+    def __pos__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="ipow"))  # TODO
-    def __pow__(self: int, other: int) -> int:
-        ...
+    def __pow__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("iadd"), ReversingChecker())
-    def __radd__(self: int, other: int) -> int:
-        ...
+    def __radd__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("rand"), ReversingChecker())
-    def __rand__(self: int, other: int) -> int:
-        ...
+    def __rand__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("idivmod_s", num_params=2), ReversingChecker())
-    def __rdivmod__(self: int, other: int) -> tuple[int, int]:
-        ...
+    def __rdivmod__(self: int, other: int) -> tuple[int, int]: ...
 
     @guppy.hugr_op(builtins, int_op("idiv_s", num_params=2), ReversingChecker())
-    def __rfloordiv__(self: int, other: int) -> int:
-        ...
+    def __rfloordiv__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(
         builtins, int_op("ishl", num_params=2), ReversingChecker()
     )  # TODO: RHS is unsigned
-    def __rlshift__(self: int, other: int) -> int:
-        ...
+    def __rlshift__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("imod_s", num_params=2), ReversingChecker())
-    def __rmod__(self: int, other: int) -> int:
-        ...
+    def __rmod__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("imul"), ReversingChecker())
-    def __rmul__(self: int, other: int) -> int:
-        ...
+    def __rmul__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ior"), ReversingChecker())
-    def __ror__(self: int, other: int) -> int:
-        ...
+    def __ror__(self: int, other: int) -> int: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __round__(self: int) -> int:
-        ...
+    def __round__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="ipow"), ReversingChecker())  # TODO
-    def __rpow__(self: int, other: int) -> int:
-        ...
+    def __rpow__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(
         builtins, int_op("ishr", num_params=2), ReversingChecker()
     )  # TODO: RHS is unsigned
-    def __rrshift__(self: int, other: int) -> int:
-        ...
+    def __rrshift__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ishr", num_params=2))  # TODO: RHS is unsigned
-    def __rshift__(self: int, other: int) -> int:
-        ...
+    def __rshift__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("isub"), ReversingChecker())
-    def __rsub__(self: int, other: int) -> int:
-        ...
+    def __rsub__(self: int, other: int) -> int: ...
 
     @guppy.custom(builtins, IntTruedivCompiler(), ReversingChecker())
-    def __rtruediv__(self: int, other: int) -> float:
-        ...
+    def __rtruediv__(self: int, other: int) -> float: ...
 
     @guppy.hugr_op(builtins, int_op("ixor"), ReversingChecker())
-    def __rxor__(self: int, other: int) -> int:
-        ...
+    def __rxor__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("isub"))
-    def __sub__(self: int, other: int) -> int:
-        ...
+    def __sub__(self: int, other: int) -> int: ...
 
     @guppy.custom(builtins, IntTruedivCompiler())
-    def __truediv__(self: int, other: int) -> float:
-        ...
+    def __truediv__(self: int, other: int) -> float: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __trunc__(self: int) -> int:
-        ...
+    def __trunc__(self: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("ixor"))
-    def __xor__(self: int, other: int) -> int:
-        ...
+    def __xor__(self: int, other: int) -> int: ...
 
 
 @guppy.type(builtins, hugr_float_type, name="float", bound=tys.TypeBound.Copyable)
 class Float:
     @guppy.hugr_op(builtins, float_op("fabs"), CoercingChecker())
-    def __abs__(self: float) -> float:
-        ...
+    def __abs__(self: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fadd"), CoercingChecker())
-    def __add__(self: float, other: float) -> float:
-        ...
+    def __add__(self: float, other: float) -> float: ...
 
     @guppy.custom(builtins, FloatBoolCompiler(), CoercingChecker())
-    def __bool__(self: float) -> bool:
-        ...
+    def __bool__(self: float) -> bool: ...
 
     @guppy.hugr_op(builtins, float_op("fceil"), CoercingChecker())
-    def __ceil__(self: float) -> float:
-        ...
+    def __ceil__(self: float) -> float: ...
 
     @guppy.custom(builtins, FloatDivmodCompiler(), CoercingChecker())
-    def __divmod__(self: float, other: float) -> tuple[float, float]:
-        ...
+    def __divmod__(self: float, other: float) -> tuple[float, float]: ...
 
     @guppy.hugr_op(builtins, float_op("feq"), CoercingChecker())
-    def __eq__(self: float, other: float) -> bool:
-        ...
+    def __eq__(self: float, other: float) -> bool: ...
 
     @guppy.custom(builtins, NoopCompiler(), CoercingChecker())
-    def __float__(self: float) -> float:
-        ...
+    def __float__(self: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("ffloor"), CoercingChecker())
-    def __floor__(self: float) -> float:
-        ...
+    def __floor__(self: float) -> float: ...
 
     @guppy.custom(builtins, FloatFloordivCompiler(), CoercingChecker())
-    def __floordiv__(self: float, other: float) -> float:
-        ...
+    def __floordiv__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fge"), CoercingChecker())
-    def __ge__(self: float, other: float) -> bool:
-        ...
+    def __ge__(self: float, other: float) -> bool: ...
 
     @guppy.hugr_op(builtins, float_op("fgt"), CoercingChecker())
-    def __gt__(self: float, other: float) -> bool:
-        ...
+    def __gt__(self: float, other: float) -> bool: ...
 
     @guppy.hugr_op(
         builtins, float_op("trunc_s", "arithmetic.conversions"), CoercingChecker()
     )
-    def __int__(self: float) -> int:
-        ...
+    def __int__(self: float) -> int: ...
 
     @guppy.hugr_op(builtins, float_op("fle"), CoercingChecker())
-    def __le__(self: float, other: float) -> bool:
-        ...
+    def __le__(self: float, other: float) -> bool: ...
 
     @guppy.hugr_op(builtins, float_op("flt"), CoercingChecker())
-    def __lt__(self: float, other: float) -> bool:
-        ...
+    def __lt__(self: float, other: float) -> bool: ...
 
     @guppy.custom(builtins, FloatModCompiler(), CoercingChecker())
-    def __mod__(self: float, other: float) -> float:
-        ...
+    def __mod__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fmul"), CoercingChecker())
-    def __mul__(self: float, other: float) -> float:
-        ...
+    def __mul__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fne"), CoercingChecker())
-    def __ne__(self: float, other: float) -> bool:
-        ...
+    def __ne__(self: float, other: float) -> bool: ...
 
     @guppy.hugr_op(builtins, float_op("fneg"), CoercingChecker())
-    def __neg__(self: float, other: float) -> float:
-        ...
+    def __neg__(self: float, other: float) -> float: ...
 
     @guppy.custom(builtins, NoopCompiler(), CoercingChecker())
-    def __pos__(self: float) -> float:
-        ...
+    def __pos__(self: float) -> float: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="fpow"))  # TODO
-    def __pow__(self: float, other: float) -> float:
-        ...
+    def __pow__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fadd"), ReversingChecker(CoercingChecker()))
-    def __radd__(self: float, other: float) -> float:
-        ...
+    def __radd__(self: float, other: float) -> float: ...
 
     @guppy.custom(builtins, FloatDivmodCompiler(), ReversingChecker(CoercingChecker()))
-    def __rdivmod__(self: float, other: float) -> tuple[float, float]:
-        ...
+    def __rdivmod__(self: float, other: float) -> tuple[float, float]: ...
 
     @guppy.custom(
         builtins, FloatFloordivCompiler(), ReversingChecker(CoercingChecker())
     )
-    def __rfloordiv__(self: float, other: float) -> float:
-        ...
+    def __rfloordiv__(self: float, other: float) -> float: ...
 
     @guppy.custom(builtins, FloatModCompiler(), ReversingChecker(CoercingChecker()))
-    def __rmod__(self: float, other: float) -> float:
-        ...
+    def __rmod__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fmul"), ReversingChecker(CoercingChecker()))
-    def __rmul__(self: float, other: float) -> float:
-        ...
+    def __rmul__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="fround"))  # TODO
-    def __round__(self: float) -> float:
-        ...
+    def __round__(self: float) -> float: ...
 
     @guppy.hugr_op(
         builtins, ops.DummyOp(name="fpow"), ReversingChecker(DefaultCallChecker())
     )  # TODO
-    def __rpow__(self: float, other: float) -> float:
-        ...
+    def __rpow__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fsub"), ReversingChecker(CoercingChecker()))
-    def __rsub__(self: float, other: float) -> float:
-        ...
+    def __rsub__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fdiv"), ReversingChecker(CoercingChecker()))
-    def __rtruediv__(self: float, other: float) -> float:
-        ...
+    def __rtruediv__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fsub"), CoercingChecker())
-    def __sub__(self: float, other: float) -> float:
-        ...
+    def __sub__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fdiv"), CoercingChecker())
-    def __truediv__(self: float, other: float) -> float:
-        ...
+    def __truediv__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(
         builtins, float_op("trunc_s", "arithmetic.conversions"), CoercingChecker()
     )
-    def __trunc__(self: float) -> float:
-        ...
+    def __trunc__(self: float) -> float: ...
 
 
-@guppy.extend_type(builtins, ListType)
+@guppy.extend_type(builtins, list_type_def)
 class List:
     @guppy.hugr_op(builtins, ops.DummyOp(name="Concat"))
-    def __add__(self: list[T], other: list[T]) -> list[T]:
-        ...
+    def __add__(self: list[T], other: list[T]) -> list[T]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="IsEmpty"))
-    def __bool__(self: list[T]) -> bool:
-        ...
+    def __bool__(self: list[T]) -> bool: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Contains"))
-    def __contains__(self: list[T], el: T) -> bool:
-        ...
+    def __contains__(self: list[T], el: T) -> bool: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="AssertEmpty"))
-    def __end__(self: list[T]) -> None:
-        ...
+    def __end__(self: list[T]) -> None: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Lookup"))
-    def __getitem__(self: list[T], idx: int) -> T:
-        ...
+    def __getitem__(self: list[T], idx: int) -> T: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="IsNonEmpty"))
-    def __hasnext__(self: list[T]) -> tuple[bool, list[T]]:
-        ...
+    def __hasnext__(self: list[T]) -> tuple[bool, list[T]]: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __iter__(self: list[T]) -> list[T]:
-        ...
+    def __iter__(self: list[T]) -> list[T]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Length"))
-    def __len__(self: list[T]) -> int:
-        ...
+    def __len__(self: list[T]) -> int: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Repeat"))
-    def __mul__(self: list[T], other: int) -> list[T]:
-        ...
+    def __mul__(self: list[T], other: int) -> list[T]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Pop"))
-    def __next__(self: list[T]) -> tuple[T, list[T]]:
-        ...
+    def __next__(self: list[T]) -> tuple[T, list[T]]: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def __setitem__(self: list[T], idx: int, value: T) -> None:
-        ...
+    def __setitem__(self: list[T], idx: int, value: T) -> None: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Append"), ReversingChecker())
-    def __radd__(self: list[T], other: list[T]) -> list[T]:
-        ...
+    def __radd__(self: list[T], other: list[T]) -> list[T]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Repeat"), ReversingChecker())
-    def __rmul__(self: list[T], other: int) -> list[T]:
-        ...
+    def __rmul__(self: list[T], other: int) -> list[T]: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def append(self: list[T], elt: T) -> None:
-        ...
+    def append(self: list[T], elt: T) -> None: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def clear(self: list[T]) -> None:
-        ...
+    def clear(self: list[T]) -> None: ...
 
     @guppy.custom(builtins, NoopCompiler())  # Can be noop since lists are immutable
-    def copy(self: list[T]) -> list[T]:
-        ...
+    def copy(self: list[T]) -> list[T]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Count"))
-    def count(self: list[T], elt: T) -> int:
-        ...
+    def count(self: list[T], elt: T) -> int: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def extend(self: list[T], seq: None) -> None:
-        ...
+    def extend(self: list[T], seq: None) -> None: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Find"))
-    def index(self: list[T], elt: T) -> int:
-        ...
+    def index(self: list[T], elt: T) -> int: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def pop(self: list[T], idx: int) -> None:
-        ...
+    def pop(self: list[T], idx: int) -> None: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def remove(self: list[T], elt: T) -> None:
-        ...
+    def remove(self: list[T], elt: T) -> None: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def reverse(self: list[T]) -> None:
-        ...
+    def reverse(self: list[T]) -> None: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def sort(self: list[T]) -> None:
-        ...
+    def sort(self: list[T]) -> None: ...
 
 
 linst = list
 
 
-@guppy.extend_type(builtins, LinstType)
+@guppy.extend_type(builtins, linst_type_def)
 class Linst:
     @guppy.hugr_op(builtins, ops.DummyOp(name="Append"))
-    def __add__(self: linst[L], other: linst[L]) -> linst[L]:
-        ...
+    def __add__(self: linst[L], other: linst[L]) -> linst[L]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="AssertEmpty"))
-    def __end__(self: linst[L]) -> None:
-        ...
+    def __end__(self: linst[L]) -> None: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="IsNonempty"))
-    def __hasnext__(self: linst[L]) -> tuple[bool, linst[L]]:
-        ...
+    def __hasnext__(self: linst[L]) -> tuple[bool, linst[L]]: ...
 
     @guppy.custom(builtins, NoopCompiler())
-    def __iter__(self: linst[L]) -> linst[L]:
-        ...
+    def __iter__(self: linst[L]) -> linst[L]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Length"))
-    def __len__(self: linst[L]) -> tuple[int, linst[L]]:
-        ...
+    def __len__(self: linst[L]) -> tuple[int, linst[L]]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Pop"))
-    def __next__(self: linst[L]) -> tuple[L, linst[L]]:
-        ...
+    def __next__(self: linst[L]) -> tuple[L, linst[L]]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Append"), ReversingChecker())
-    def __radd__(self: linst[L], other: linst[L]) -> linst[L]:
-        ...
+    def __radd__(self: linst[L], other: linst[L]) -> linst[L]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Repeat"), ReversingChecker())
-    def __rmul__(self: linst[L], other: int) -> linst[L]:
-        ...
+    def __rmul__(self: linst[L], other: int) -> linst[L]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Push"))
-    def append(self: linst[L], elt: L) -> linst[L]:
-        ...
+    def append(self: linst[L], elt: L) -> linst[L]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="PopAt"))
-    def pop(self: linst[L], idx: int) -> tuple[L, linst[L]]:
-        ...
+    def pop(self: linst[L], idx: int) -> tuple[L, linst[L]]: ...
 
     @guppy.hugr_op(builtins, ops.DummyOp(name="Reverse"))
-    def reverse(self: linst[L]) -> linst[L]:
-        ...
+    def reverse(self: linst[L]) -> linst[L]: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
-    def sort(self: list[T]) -> None:
-        ...
+    def sort(self: list[T]) -> None: ...
 
 
 @guppy.custom(builtins, checker=DunderChecker("__abs__"), higher_order_value=False)
-def abs(x):
-    ...
+def abs(x): ...
 
 
 @guppy.custom(
     builtins, name="bool", checker=DunderChecker("__bool__"), higher_order_value=False
 )
-def _bool(x):
-    ...
+def _bool(x): ...
 
 
 @guppy.custom(builtins, checker=CallableChecker(), higher_order_value=False)
-def callable(x):
-    ...
+def callable(x): ...
 
 
 @guppy.custom(
     builtins, checker=DunderChecker("__divmod__", num_args=2), higher_order_value=False
 )
-def divmod(x, y):
-    ...
+def divmod(x, y): ...
 
 
 @guppy.custom(
     builtins, name="float", checker=DunderChecker("__float__"), higher_order_value=False
 )
-def _float(x, y):
-    ...
+def _float(x, y): ...
 
 
 @guppy.custom(
     builtins, name="int", checker=DunderChecker("__int__"), higher_order_value=False
 )
-def _int(x):
-    ...
+def _int(x): ...
 
 
 @guppy.custom(builtins, checker=DunderChecker("__len__"), higher_order_value=False)
-def len(x):
-    ...
+def len(x): ...
 
 
 @guppy.custom(
     builtins, checker=DunderChecker("__pow__", num_args=2), higher_order_value=False
 )
-def pow(x, y):
-    ...
+def pow(x, y): ...
 
 
 @guppy.custom(builtins, checker=DunderChecker("__round__"), higher_order_value=False)
-def round(x):
-    ...
+def round(x): ...
 
 
 # Python builtins that are not supported yet:
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def aiter(x):
-    ...
+def aiter(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def all(x):
-    ...
+def all(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def anext(x):
-    ...
+def anext(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def any(x):
-    ...
+def any(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def bin(x):
-    ...
+def bin(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def breakpoint(x):
-    ...
+def breakpoint(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def bytearray(x):
-    ...
+def bytearray(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def bytes(x):
-    ...
+def bytes(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def chr(x):
-    ...
+def chr(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def classmethod(x):
-    ...
+def classmethod(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def compile(x):
-    ...
+def compile(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def complex(x):
-    ...
+def complex(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def delattr(x):
-    ...
+def delattr(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def dict(x):
-    ...
+def dict(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def dir(x):
-    ...
+def dir(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def enumerate(x):
-    ...
+def enumerate(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def eval(x):
-    ...
+def eval(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def exec(x):
-    ...
+def exec(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def filter(x):
-    ...
+def filter(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def format(x):
-    ...
+def format(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def forozenset(x):
-    ...
+def forozenset(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def getattr(x):
-    ...
+def getattr(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def globals():
-    ...
+def globals(): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def hasattr(x):
-    ...
+def hasattr(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def hash(x):
-    ...
+def hash(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def help(x):
-    ...
+def help(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def hex(x):
-    ...
+def hex(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def id(x):
-    ...
+def id(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def input(x):
-    ...
+def input(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def isinstance(x):
-    ...
+def isinstance(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def issubclass(x):
-    ...
+def issubclass(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def iter(x):
-    ...
+def iter(x): ...
 
 
 @guppy.custom(
     builtins, checker=UnsupportedChecker(), name="list", higher_order_value=False
 )
-def _list(x):
-    ...
+def _list(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def locals(x):
-    ...
+def locals(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def map(x):
-    ...
+def map(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def max(x):
-    ...
+def max(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def memoryview(x):
-    ...
+def memoryview(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def min(x):
-    ...
+def min(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def next(x):
-    ...
+def next(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def object(x):
-    ...
+def object(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def oct(x):
-    ...
+def oct(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def open(x):
-    ...
+def open(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def ord(x):
-    ...
+def ord(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def print(x):
-    ...
+def print(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def property(x):
-    ...
+def property(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def range(x):
-    ...
+def range(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def repr(x):
-    ...
+def repr(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def reversed(x):
-    ...
+def reversed(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def set(x):
-    ...
+def set(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def setattr(x):
-    ...
+def setattr(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def slice(x):
-    ...
+def slice(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def sorted(x):
-    ...
+def sorted(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def staticmethod(x):
-    ...
+def staticmethod(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def str(x):
-    ...
+def str(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def sum(x):
-    ...
+def sum(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def super(x):
-    ...
+def super(x): ...
 
 
 @guppy.custom(
     builtins, name="tuple", checker=UnsupportedChecker(), higher_order_value=False
 )
-def _tuple(x):
-    ...
+def _tuple(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def type(x):
-    ...
+def type(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def vars(x):
-    ...
+def vars(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def zip(x):
-    ...
+def zip(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
-def __import__(x):
-    ...
+def __import__(x): ...
```

### Comparing `guppylang-0.1.0/guppylang/prelude/quantum.py` & `guppylang-0.2.0/guppylang/prelude/quantum.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,114 +17,93 @@
 
 
 @guppy.type(
     quantum,
     tys.Opaque(extension="prelude", id="qubit", args=[], bound=TypeBound.Any),
     linear=True,
 )
-class Qubit:
+class qubit:
     pass
 
 
 @guppy.hugr_op(quantum, quantum_op("H"))
-def h(q: Qubit) -> Qubit:
-    ...
+def h(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("CZ"))
-def cz(control: Qubit, target: Qubit) -> tuple[Qubit, Qubit]:
-    ...
+def cz(control: qubit, target: qubit) -> tuple[qubit, qubit]: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("CX"))
-def cx(control: Qubit, target: Qubit) -> tuple[Qubit, Qubit]:
-    ...
+def cx(control: qubit, target: qubit) -> tuple[qubit, qubit]: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("T"))
-def t(q: Qubit) -> Qubit:
-    ...
+def t(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("S"))
-def s(q: Qubit) -> Qubit:
-    ...
+def s(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("X"))
-def x(q: Qubit) -> Qubit:
-    ...
+def x(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Y"))
-def y(q: Qubit) -> Qubit:
-    ...
+def y(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Z"))
-def z(q: Qubit) -> Qubit:
-    ...
+def z(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Tdg"))
-def tdg(q: Qubit) -> Qubit:
-    ...
+def tdg(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Sdg"))
-def sdg(q: Qubit) -> Qubit:
-    ...
+def sdg(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("ZZMax"))
-def zz_max(q: Qubit) -> Qubit:
-    ...
+def zz_max(q1: qubit, q2: qubit) -> tuple[qubit, qubit]: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Measure"))
-def measure_return(q: Qubit) -> tuple[Qubit, bool]:
-    ...
+def measure_return(q: qubit) -> tuple[qubit, bool]: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("RzF64"))
-def rz(q: Qubit, angle: float) -> Qubit:
-    ...
+def rz(q: qubit, angle: float) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("RxF64"))
-def rx(q: Qubit, angle: float) -> Qubit:
-    ...
+def rx(q: qubit, angle: float) -> qubit: ...
 
 
-@guppy.hugr_op(quantum, quantum_op("RzF64"))
-def phased_x(q: Qubit, angle1: float, angle2: float) -> Qubit:
-    ...
+@guppy.hugr_op(quantum, quantum_op("PhasedX"))
+def phased_x(q: qubit, angle1: float, angle2: float) -> qubit: ...
 
 
-@guppy.hugr_op(quantum, quantum_op("RzF64"))
-def zz_phase(q1: Qubit, q2: Qubit, angle: float) -> tuple[Qubit, Qubit]:
-    ...
+@guppy.hugr_op(quantum, quantum_op("ZZPhase"))
+def zz_phase(q1: qubit, q2: qubit, angle: float) -> tuple[qubit, qubit]: ...
 
 
-@guppy.hugr_op(quantum, quantum_op("RzF64"))
-def tk1(q: Qubit, angle1: float, angle2: float, angle3: float) -> Qubit:
-    ...
+@guppy.hugr_op(quantum, quantum_op("TK1"))
+def tk1(q: qubit, angle1: float, angle2: float, angle3: float) -> qubit: ...
 
 
-@guppy.hugr_op(quantum, quantum_op("QAlloc"), name="Qubit")
-def _Qubit() -> Qubit:
-    ...
+@guppy.hugr_op(quantum, quantum_op("QAlloc"), name="qubit")
+def _qubit() -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("QFree"))
-def discard(q: Qubit) -> None:
-    ...
+def discard(q: qubit) -> None: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Reset"))
-def reset(q: Qubit) -> Qubit:
-    ...
+def reset(q: qubit) -> qubit: ...
 
 
 @guppy.custom(quantum, MeasureCompiler())
-def measure(q: Qubit) -> bool:
-    ...
+def measure(q: qubit) -> bool: ...
```

### Comparing `guppylang-0.1.0/pyproject.toml` & `guppylang-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "guppylang"
-version = "0.1.0"
-description = ""
+version = "0.2.0"
+description = "Pythonic quantum-classical programming language"
 authors = ["Mark Koch <mark.koch@quantinuum.com>"]
 license = "Apache-2.0"
-readme = "README.md"
+readme = "quickstart.md"
 repository = "https://github.com/CQCL/guppy"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 graphviz = "^0.20.1"
 networkx = "^3.2.1"
-pydantic = "^2.5.3"
+pydantic = "^2.7.0b1"
 typing-extensions = "^4.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
+pytest-cov = "^4.1.0"
 mypy = "^1.8.0"
 pre-commit = "^3.6.0"
-ruff = "^0.1.11"
+ruff = ">=0.3"
 maturin = "^1.4.0"
 pytket = "*"
 
 [tool.poetry.group.validation]
 optional = true
 
 [tool.poetry.group.validation.dependencies]
@@ -30,15 +31,15 @@
 
 
 [tool.poetry.group.pytket]
 optional = true
 
 [tool.poetry.group.pytket.dependencies]
 pytket = { version = "^1.24.0" }
-tket2-py = {git = "https://github.com/CQCL/tket2.git", rev = "9e941f3"}
+tket2-py = { git = "https://github.com/CQCL/tket2.git", rev = "9e941f3" }
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

