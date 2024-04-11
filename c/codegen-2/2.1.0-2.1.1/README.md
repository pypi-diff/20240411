# Comparing `tmp/codegen_2-2.1.0.tar.gz` & `tmp/codegen_2-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegen_2-2.1.0.tar", max compression
+gzip compressed data, was "codegen_2-2.1.1.tar", max compression
```

## Comparing `codegen_2-2.1.0.tar` & `codegen_2-2.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2024-03-22 01:07:01.506500 codegen_2-2.1.0/LICENSE
--rw-r--r--   0        0        0       27 2024-03-22 01:07:01.506500 codegen_2-2.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/__init__.py
--rw-r--r--   0        0        0      457 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/__init__.py
--rw-r--r--   0        0        0     7678 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/ast.py
--rw-r--r--   0        0        0     4825 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/expr.py
--rw-r--r--   0        0        0     4471 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/program.py
--rw-r--r--   0        0        0     2899 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/statement.py
--rw-r--r--   0        0        0      178 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/types.py
--rw-r--r--   0        0        0     1771 2024-03-22 01:07:01.506500 codegen_2-2.1.0/codegen/models/var.py
--rw-r--r--   0        0        0      422 2024-03-22 01:07:01.506500 codegen_2-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 codegen_2-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-11 00:16:20.368382 codegen_2-2.1.1/LICENSE
+-rw-r--r--   0        0        0       27 2024-04-11 00:16:20.368382 codegen_2-2.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/__init__.py
+-rw-r--r--   0        0        0     7702 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/ast.py
+-rw-r--r--   0        0        0     5273 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/expr.py
+-rw-r--r--   0        0        0     4471 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/program.py
+-rw-r--r--   0        0        0     2899 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/statement.py
+-rw-r--r--   0        0        0      178 2024-04-11 00:16:20.372382 codegen_2-2.1.1/codegen/models/types.py
+-rw-r--r--   0        0        0     1771 2024-04-11 00:16:20.372382 codegen_2-2.1.1/codegen/models/var.py
+-rw-r--r--   0        0        0      422 2024-04-11 00:16:20.372382 codegen_2-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 codegen_2-2.1.1/PKG-INFO
```

### Comparing `codegen_2-2.1.0/LICENSE` & `codegen_2-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.0/codegen/models/ast.py` & `codegen_2-2.1.1/codegen/models/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,17 @@
 
         return self._add_stmt(ForLoopStatement(var, iter))
 
     def if_(self, condition: Expr):
         return self._add_stmt(IfStatement(condition))
 
     def else_(self):
-        assert len(self.children) > 0 and isinstance(self.children[-1].stmt, Statement)
+        assert len(self.children) > 0 and isinstance(
+            self.children[-1].stmt, IfStatement
+        )
         return self._add_stmt(ElseStatement())
 
     def python_stmt(self, stmt: str) -> AST:
         return self._add_stmt(PythonStatement(stmt))
 
     def update_recursively(
         self, fn: Callable[[AST, Any], tuple[AST, Any, bool]], context: Any
```

### Comparing `codegen_2-2.1.0/codegen/models/expr.py` & `codegen_2-2.1.1/codegen/models/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,17 @@
 
 
 @dataclass
 class ExprNegation(Expr):
     expr: Expr
 
     def to_python(self):
-        return f"not {self.expr.to_python()}"
+        if isinstance(self.expr, (ExprVar, ExprConstant)):
+            return f"not {self.expr.to_python()}"
+        return f"not ({self.expr.to_python()})"
 
 
 class PredefinedFn:
     @dataclass
     class tuple(Expr):
         items: Sequence[Expr]
 
@@ -169,15 +171,25 @@
 
     @dataclass
     class set_contains(Expr):
         set_: Expr
         item: Expr
 
         def to_python(self):
-            return f"({self.item.to_python()}) in {self.set_.to_python()}"
+            if isinstance(self.set_, (ExprVar, ExprConstant)):
+                set_py = self.set_.to_python()
+            else:
+                set_py = f"({self.set_.to_python()})"
+
+            if isinstance(self.item, (ExprVar, ExprConstant)):
+                item_py = self.item.to_python()
+            else:
+                item_py = f"({self.item.to_python()})"
+
+            return f"{item_py} in {set_py}"
 
     @dataclass
     class list_append(Expr):
         lst: Expr
         item: Expr
 
         def to_python(self):
```

### Comparing `codegen_2-2.1.0/codegen/models/program.py` & `codegen_2-2.1.1/codegen/models/program.py`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.0/codegen/models/statement.py` & `codegen_2-2.1.1/codegen/models/statement.py`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.0/codegen/models/var.py` & `codegen_2-2.1.1/codegen/models/var.py`

 * *Files identical despite different names*

