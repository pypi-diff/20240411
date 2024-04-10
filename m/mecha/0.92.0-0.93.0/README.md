# Comparing `tmp/mecha-0.92.0.tar.gz` & `tmp/mecha-0.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecha-0.92.0.tar", max compression
+gzip compressed data, was "mecha-0.93.0.tar", max compression
```

## Comparing `mecha-0.92.0.tar` & `mecha-0.93.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1073 2024-04-03 07:25:04.503241 mecha-0.92.0/LICENSE
--rw-r--r--   0        0        0     8612 2024-04-03 07:25:04.503241 mecha-0.92.0/README.md
--rw-r--r--   0        0        0      344 2024-04-03 07:25:31.739479 mecha-0.92.0/mecha/__init__.py
--rw-r--r--   0        0        0       35 2024-04-03 07:25:04.511241 mecha-0.92.0/mecha/__main__.py
--rw-r--r--   0        0        0    22660 2024-04-03 07:25:04.511241 mecha-0.92.0/mecha/api.py
--rw-r--r--   0        0        0    35409 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/ast.py
--rw-r--r--   0        0        0     3057 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/cli.py
--rw-r--r--   0        0        0      719 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/commands.py
--rw-r--r--   0        0        0     6147 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/config.py
--rw-r--r--   0        0        0        0 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/annotate_diagnostics.py
--rw-r--r--   0        0        0    12498 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/bake_macros.py
--rw-r--r--   0        0        0      177 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/clear_diagnostics.py
--rw-r--r--   0        0        0     1096 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/debug_ast.py
--rw-r--r--   0        0        0     5840 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/embed.py
--rw-r--r--   0        0        0     2932 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/implicit_execute.py
--rw-r--r--   0        0        0     2592 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     6358 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/json_files.py
--rw-r--r--   0        0        0     2561 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/lint_basic.py
--rw-r--r--   0        0        0     2678 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/messages.py
--rw-r--r--   0        0        0     6188 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/nested_location.py
--rw-r--r--   0        0        0    12727 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/nested_resources.py
--rw-r--r--   0        0        0     9514 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/nested_yaml.py
--rw-r--r--   0        0        0    15453 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/nesting.py
--rw-r--r--   0        0        0     1050 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/raw.py
--rw-r--r--   0        0        0     2468 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/relative_location.py
--rw-r--r--   0        0        0     2234 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/source_map.py
--rw-r--r--   0        0        0    11944 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/statistics.py
--rw-r--r--   0        0        0       21 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/validation/__init__.py
--rw-r--r--   0        0        0    38232 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/contrib/validation/mcdoc.py
--rw-r--r--   0        0        0     6205 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/database.py
--rw-r--r--   0        0        0     5964 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/diagnostic.py
--rw-r--r--   0        0        0    13332 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/dispatch.py
--rw-r--r--   0        0        0      106 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/error.py
--rw-r--r--   0        0        0    69515 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/parse.py
--rw-r--r--   0        0        0      205 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/plugin.py
--rw-r--r--   0        0        0     1181 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/preprocess.py
--rw-r--r--   0        0        0     1214 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/prototype.py
--rw-r--r--   0        0        0        0 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/py.typed
--rw-r--r--   0        0        0   257142 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/resources/1_16.json
--rw-r--r--   0        0        0   266016 2024-04-03 07:25:04.515241 mecha-0.92.0/mecha/resources/1_17.json
--rw-r--r--   0        0        0   265402 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/1_18.json
--rw-r--r--   0        0        0   393608 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/1_19.json
--rw-r--r--   0        0        0   392539 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/1_20.json
--rw-r--r--   0        0        0        0 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/__init__.py
--rw-r--r--   0        0        0      369 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/inline_function_tag.json
--rw-r--r--   0        0        0     7984 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/nesting.json
--rw-r--r--   0        0        0      526 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/resources/patches.json
--rw-r--r--   0        0        0    11323 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/serialize.py
--rw-r--r--   0        0        0     3440 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/spec.py
--rw-r--r--   0        0        0     6393 2024-04-03 07:25:04.519241 mecha-0.92.0/mecha/utils.py
--rw-r--r--   0        0        0     1293 2024-04-03 07:25:31.767479 mecha-0.92.0/pyproject.toml
--rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 mecha-0.92.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-10 23:45:24.453071 mecha-0.93.0/LICENSE
+-rw-r--r--   0        0        0     8612 2024-04-10 23:45:24.453071 mecha-0.93.0/README.md
+-rw-r--r--   0        0        0      344 2024-04-10 23:45:44.416932 mecha-0.93.0/mecha/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-10 23:45:24.461071 mecha-0.93.0/mecha/__main__.py
+-rw-r--r--   0        0        0    22660 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/api.py
+-rw-r--r--   0        0        0    36695 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/ast.py
+-rw-r--r--   0        0        0     3057 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/cli.py
+-rw-r--r--   0        0        0      719 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/commands.py
+-rw-r--r--   0        0        0     6147 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/config.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/annotate_diagnostics.py
+-rw-r--r--   0        0        0    12498 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/bake_macros.py
+-rw-r--r--   0        0        0      177 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/clear_diagnostics.py
+-rw-r--r--   0        0        0     1096 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/debug_ast.py
+-rw-r--r--   0        0        0     5840 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/embed.py
+-rw-r--r--   0        0        0     2932 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/implicit_execute.py
+-rw-r--r--   0        0        0     2592 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     6358 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/json_files.py
+-rw-r--r--   0        0        0     2561 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/lint_basic.py
+-rw-r--r--   0        0        0     2678 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/messages.py
+-rw-r--r--   0        0        0     6188 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/nested_location.py
+-rw-r--r--   0        0        0    12727 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/nested_resources.py
+-rw-r--r--   0        0        0     9514 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/nested_yaml.py
+-rw-r--r--   0        0        0    15453 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/nesting.py
+-rw-r--r--   0        0        0     1050 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/raw.py
+-rw-r--r--   0        0        0     2468 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/relative_location.py
+-rw-r--r--   0        0        0     2234 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/source_map.py
+-rw-r--r--   0        0        0    11944 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/statistics.py
+-rw-r--r--   0        0        0       21 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/validation/__init__.py
+-rw-r--r--   0        0        0    38232 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/contrib/validation/mcdoc.py
+-rw-r--r--   0        0        0     6205 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/database.py
+-rw-r--r--   0        0        0     5964 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/diagnostic.py
+-rw-r--r--   0        0        0    13332 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/dispatch.py
+-rw-r--r--   0        0        0      106 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/error.py
+-rw-r--r--   0        0        0    72706 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/parse.py
+-rw-r--r--   0        0        0      205 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/plugin.py
+-rw-r--r--   0        0        0     1181 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/preprocess.py
+-rw-r--r--   0        0        0     1214 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/prototype.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/py.typed
+-rw-r--r--   0        0        0   257142 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/resources/1_16.json
+-rw-r--r--   0        0        0   266016 2024-04-10 23:45:24.465071 mecha-0.93.0/mecha/resources/1_17.json
+-rw-r--r--   0        0        0   265402 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/1_18.json
+-rw-r--r--   0        0        0   393608 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/1_19.json
+-rw-r--r--   0        0        0   392539 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/1_20.json
+-rw-r--r--   0        0        0        0 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/inline_function_tag.json
+-rw-r--r--   0        0        0     7984 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/nesting.json
+-rw-r--r--   0        0        0      526 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/resources/patches.json
+-rw-r--r--   0        0        0    12620 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/serialize.py
+-rw-r--r--   0        0        0     3440 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/spec.py
+-rw-r--r--   0        0        0     6393 2024-04-10 23:45:24.469071 mecha-0.93.0/mecha/utils.py
+-rw-r--r--   0        0        0     1293 2024-04-10 23:45:44.440932 mecha-0.93.0/pyproject.toml
+-rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 mecha-0.93.0/PKG-INFO
```

### Comparing `mecha-0.92.0/LICENSE` & `mecha-0.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/README.md` & `mecha-0.93.0/README.md`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/api.py` & `mecha-0.93.0/mecha/api.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/ast.py` & `mecha-0.93.0/mecha/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,19 @@
     "AstNbtByteArray",
     "AstNbtIntArray",
     "AstNbtLongArray",
     "AstResourceLocation",
     "AstBlockState",
     "AstBlock",
     "AstItemComponent",
-    "AstItem",
+    "AstItemStack",
+    "AstItemPredicateTestComponent",
+    "AstItemPredicateTestPredicate",
+    "AstItemPredicateAlternatives",
+    "AstItemPredicate",
     "AstItemSlot",
     "AstItemSlots",
     "AstRange",
     "AstTime",
     "AstSelectorScoreMatch",
     "AstSelectorScores",
     "AstSelectorAdvancementPredicateMatch",
@@ -910,20 +914,56 @@
     """Ast item component node."""
 
     key: AstResourceLocation = required_field()
     value: AstNbt = required_field()
 
 
 @dataclass(frozen=True, slots=True)
-class AstItem(AstNode):
-    """Ast item node."""
+class AstItemStack(AstNode):
+    """Ast item stack node."""
 
     identifier: AstResourceLocation = required_field()
-    components: AstChildren[AstItemComponent] = AstChildren()
-    data_tags: Optional[AstNbtCompound] = None
+    arguments: AstChildren[AstItemComponent] = AstChildren()
+    data_tags: Optional[AstNbtCompound] = None  # legacy compat
+
+
+@dataclass(frozen=True, slots=True)
+class AstItemPredicateTestComponent(AstNode):
+    """Ast item predicate test component node."""
+
+    inverted: bool = False
+    key: AstResourceLocation = required_field()
+    value: Optional[AstNbt] = None
+
+
+@dataclass(frozen=True, slots=True)
+class AstItemPredicateTestPredicate(AstNode):
+    """Ast item predicate test predicate node."""
+
+    inverted: bool = False
+    key: AstResourceLocation = required_field()
+    value: AstNbt = required_field()
+
+
+@dataclass(frozen=True, slots=True)
+class AstItemPredicateAlternatives(AstNode):
+    """Ast item predicate alternatives node."""
+
+    alternatives: AstChildren[
+        Union[AstItemPredicateTestComponent, AstItemPredicateTestPredicate]
+    ] = required_field()
+
+
+@dataclass(frozen=True, slots=True)
+class AstItemPredicate(AstNode):
+    """Ast item predicate node."""
+
+    identifier: Union[AstResourceLocation, AstWildcard] = required_field()
+    arguments: AstChildren[AstItemPredicateAlternatives] = AstChildren()
+    data_tags: Optional[AstNbtCompound] = None  # legacy compat
 
 
 @dataclass(frozen=True, slots=True)
 class AstItemSlot(AstOption):
     """Ast item slot node."""
 
     parser = "item_slot"
@@ -1189,15 +1229,15 @@
 
         if not components:
             raise ValueError("Empty nbt path not allowed.")
         return AstNbtPath(components=AstChildren(components))
 
 
 @dataclass(frozen=True, slots=True)
-class AstParticleParameters(AstNode):
+class AstParticleParameters(AstNode):  # legacy compat
     """Base ast node for particle parameters."""
 
 
 @dataclass(frozen=True, slots=True)
 class AstDustParticleParameters(AstParticleParameters):
     """Ast dust particle parameters node."""
 
@@ -1234,15 +1274,15 @@
     block: AstBlock = required_field()
 
 
 @dataclass(frozen=True, slots=True)
 class AstItemParticleParameters(AstParticleParameters):
     """Ast item particle parameters node."""
 
-    item: AstItem = required_field()
+    item: AstItemStack = required_field()
 
 
 @dataclass(frozen=True, slots=True)
 class AstVibrationParticleParameters(AstParticleParameters):
     """Ast vibration particle parameters node."""
 
     destination_x: AstNumber = required_field()
@@ -1273,15 +1313,15 @@
 
 
 @dataclass(frozen=True, slots=True)
 class AstParticle(AstNode):
     """Ast particle node."""
 
     name: AstResourceLocation = required_field()
-    parameters: Optional[AstParticleParameters] = None
+    parameters: Optional[Union[AstParticleParameters, AstNbtCompound]] = None
 
     parser = "particle"
 
 
 @dataclass(frozen=True, slots=True)
 class AstMacroLineText(AstLiteral):
     """Ast macro line text node."""
```

### Comparing `mecha-0.92.0/mecha/cli.py` & `mecha-0.93.0/mecha/cli.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/commands.py` & `mecha-0.93.0/mecha/commands.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/config.py` & `mecha-0.93.0/mecha/config.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/annotate_diagnostics.py` & `mecha-0.93.0/mecha/contrib/annotate_diagnostics.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/bake_macros.py` & `mecha-0.93.0/mecha/contrib/bake_macros.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/debug_ast.py` & `mecha-0.93.0/mecha/contrib/debug_ast.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/embed.py` & `mecha-0.93.0/mecha/contrib/embed.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/implicit_execute.py` & `mecha-0.93.0/mecha/contrib/implicit_execute.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/inline_function_tag.py` & `mecha-0.93.0/mecha/contrib/inline_function_tag.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/json_files.py` & `mecha-0.93.0/mecha/contrib/json_files.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/lint_basic.py` & `mecha-0.93.0/mecha/contrib/lint_basic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/messages.py` & `mecha-0.93.0/mecha/contrib/messages.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/nested_location.py` & `mecha-0.93.0/mecha/contrib/nested_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/nested_resources.py` & `mecha-0.93.0/mecha/contrib/nested_resources.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/nested_yaml.py` & `mecha-0.93.0/mecha/contrib/nested_yaml.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/nesting.py` & `mecha-0.93.0/mecha/contrib/nesting.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/raw.py` & `mecha-0.93.0/mecha/contrib/raw.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/relative_location.py` & `mecha-0.93.0/mecha/contrib/relative_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/source_map.py` & `mecha-0.93.0/mecha/contrib/source_map.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/statistics.py` & `mecha-0.93.0/mecha/contrib/statistics.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/contrib/validation/mcdoc.py` & `mecha-0.93.0/mecha/contrib/validation/mcdoc.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/database.py` & `mecha-0.93.0/mecha/database.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/diagnostic.py` & `mecha-0.93.0/mecha/diagnostic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/dispatch.py` & `mecha-0.93.0/mecha/dispatch.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/parse.py` & `mecha-0.93.0/mecha/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,18 @@
     "JsonObjectParser",
     "NbtParser",
     "NbtCompoundParser",
     "AdjacentConstraint",
     "ResourceLocationParser",
     "NoTagConstraint",
     "BlockParser",
-    "BracketedKeyValuePairsParser",
+    "BracketedListParser",
+    "KeyValuePairParser",
     "ItemParser",
+    "ItemPredicateAlternativesParser",
     "NoDataTagsConstraint",
     "BasicLiteralParser",
     "RangeParser",
     "IntegerRangeConstraint",
     "LengthConstraint",
     "CommentDisambiguation",
     "TimeParser",
@@ -52,15 +54,15 @@
     "SelectorTypeConstraint",
     "SelectorSingleConstraint",
     "SelectorAmountConstraint",
     "EntityParser",
     "parse_wildcard",
     "parse_message",
     "NbtPathParser",
-    "parse_particle",
+    "ParticleParser",
     "AggregateParser",
     "SingleLineConstraint",
     "AlternativeParser",
     "NUMBER_PATTERN",
     "JSON_STRING_PATTERN",
     "NBT_QUOTED_STRING_PATTERN",
 ]
@@ -104,19 +106,23 @@
     AstDustColorTransitionParticleParameters,
     AstDustParticleParameters,
     AstEntityAnchor,
     AstFallingDustParticleParameters,
     AstGamemode,
     AstGreedy,
     AstHeightmap,
-    AstItem,
     AstItemComponent,
     AstItemParticleParameters,
+    AstItemPredicate,
+    AstItemPredicateAlternatives,
+    AstItemPredicateTestComponent,
+    AstItemPredicateTestPredicate,
     AstItemSlot,
     AstItemSlots,
+    AstItemStack,
     AstJson,
     AstJsonArray,
     AstJsonObject,
     AstJsonObjectEntry,
     AstJsonObjectKey,
     AstJsonValue,
     AstLegacyScoreboardSlot,
@@ -222,14 +228,17 @@
             integer_parser=delegate("integer"),
             nbt_compound_parser=delegate("nbt_compound"),
         ),
         "range": RangeParser(),
         "integer_range": IntegerRangeConstraint(delegate("range")),
         "resource_location_or_tag": CommentDisambiguation(ResourceLocationParser()),
         "resource_location": NoTagConstraint(delegate("resource_location_or_tag")),
+        "resource_location_or_nbt": AlternativeParser(
+            [delegate("resource_location"), delegate("nbt_compound")]
+        ),
         "uuid": parse_uuid,
         "objective": BasicLiteralParser(AstObjective),
         "objective_criteria": BasicLiteralParser(AstObjectiveCriteria),
         "scoreboard_operation": BasicLiteralParser(AstScoreboardOperation),
         "player_name": CommentDisambiguation(BasicLiteralParser(AstPlayerName)),
         "scoreboard_slot": BasicLiteralParser(AstScoreboardSlot),
         "swizzle": BasicLiteralParser(AstSwizzle),
@@ -244,62 +253,73 @@
         "entity_anchor": BasicLiteralParser(AstEntityAnchor),
         "template_rotation": BasicLiteralParser(AstTemplateRotation),
         "template_mirror": BasicLiteralParser(AstTemplateMirror),
         "block_predicate": BlockParser(
             resource_location_parser=delegate("resource_location_or_tag"),
             block_states_parser=AdjacentConstraint(
                 parser=MultilineParser(
-                    BracketedKeyValuePairsParser(
-                        node_type=AstBlockState,
-                        key_parser=StringParser(type="phrase"),
-                        value_parser=delegate("phrase"),
+                    BracketedListParser(
+                        KeyValuePairParser(
+                            node_type=AstBlockState,
+                            key_parser=StringParser(type="phrase"),
+                            value_parser=delegate("phrase"),
+                        )
                     )
                 ),
                 hint=r"\[",
             ),
             data_tags_parser=delegate("adjacent_nbt_compound"),
         ),
         "block_state": BlockParser(
             resource_location_parser=delegate("resource_location"),
             block_states_parser=AdjacentConstraint(
                 parser=MultilineParser(
-                    BracketedKeyValuePairsParser(
-                        node_type=AstBlockState,
-                        key_parser=StringParser(type="phrase"),
-                        value_parser=delegate("phrase"),
+                    BracketedListParser(
+                        KeyValuePairParser(
+                            node_type=AstBlockState,
+                            key_parser=StringParser(type="phrase"),
+                            value_parser=delegate("phrase"),
+                        )
                     )
                 ),
                 hint=r"\[",
             ),
             data_tags_parser=delegate("adjacent_nbt_compound"),
         ),
         "item_predicate": ItemParser(
-            resource_location_parser=delegate("resource_location_or_tag"),
-            components_parser=AdjacentConstraint(
+            node_type=AstItemPredicate,
+            identifier_parser=AlternativeParser(
+                [delegate("resource_location_or_tag"), delegate("wildcard")]
+            ),
+            arguments_parser=AdjacentConstraint(
                 parser=MultilineParser(
-                    BracketedKeyValuePairsParser(
-                        node_type=AstItemComponent,
-                        key_parser=delegate("resource_location"),
-                        value_parser=delegate("nbt"),
+                    BracketedListParser(
+                        ItemPredicateAlternativesParser(
+                            key_parser=delegate("resource_location"),
+                            value_parser=delegate("nbt"),
+                        )
                     )
                 ),
                 hint=r"\[",
             ),
             data_tags_parser=delegate("adjacent_nbt_compound"),
         ),
         "item_slot": BasicLiteralParser(AstItemSlot),
         "item_slots": BasicLiteralParser(AstItemSlots),
         "item_stack": ItemParser(
-            resource_location_parser=delegate("resource_location"),
-            components_parser=AdjacentConstraint(
+            node_type=AstItemStack,
+            identifier_parser=delegate("resource_location"),
+            arguments_parser=AdjacentConstraint(
                 parser=MultilineParser(
-                    BracketedKeyValuePairsParser(
-                        node_type=AstItemComponent,
-                        key_parser=delegate("resource_location"),
-                        value_parser=delegate("nbt"),
+                    BracketedListParser(
+                        KeyValuePairParser(
+                            node_type=AstItemComponent,
+                            key_parser=delegate("resource_location"),
+                            value_parser=delegate("nbt"),
+                        )
                     )
                 ),
                 hint=r"\[",
             ),
             data_tags_parser=delegate("adjacent_nbt_compound"),
         ),
         "message": parse_message,
@@ -331,15 +351,18 @@
         ),
         "game_profile": EntityParser(
             selector_parser=SelectorPlayerConstraint(delegate("selector")),
         ),
         ################################################################################
         # Particle
         ################################################################################
-        "particle": parse_particle,
+        "particle": ParticleParser(
+            resource_location_parser=delegate("resource_location"),
+            generic_parameters_parser=delegate("nbt_compound"),
+        ),
         "particle:minecraft:dust": AggregateParser(
             type=AstDustParticleParameters,
             fields={
                 "red": delegate("numeric"),
                 "green": delegate("numeric"),
                 "blue": delegate("numeric"),
                 "size": delegate("numeric"),
@@ -467,17 +490,21 @@
         "command:argument:minecraft:entity": delegate("entity"),
         "command:argument:minecraft:entity_anchor": delegate("entity_anchor"),
         "command:argument:minecraft:entity_summon": delegate("resource_location"),
         "command:argument:minecraft:template_rotation": delegate("template_rotation"),
         "command:argument:minecraft:template_mirror": delegate("template_mirror"),
         "command:argument:minecraft:float_range": delegate("range"),
         "command:argument:minecraft:function": delegate("resource_location_or_tag"),
-        "command:argument:minecraft:loot_table": delegate("resource_location"),
-        "command:argument:minecraft:loot_predicate": delegate("resource_location"),
-        "command:argument:minecraft:loot_modifier": delegate("resource_location"),
+        "command:argument:minecraft:loot_table": delegate("resource_location_or_nbt"),
+        "command:argument:minecraft:loot_predicate": delegate(
+            "resource_location_or_nbt"
+        ),
+        "command:argument:minecraft:loot_modifier": delegate(
+            "resource_location_or_nbt"
+        ),
         "command:argument:minecraft:game_profile": delegate("game_profile"),
         "command:argument:minecraft:gamemode": delegate("gamemode"),
         "command:argument:minecraft:heightmap": delegate("heightmap"),
         "command:argument:minecraft:int_range": delegate("integer_range"),
         "command:argument:minecraft:item_enchantment": delegate("word"),
         "command:argument:minecraft:item_predicate": MultilineParser(
             delegate("item_predicate")
@@ -1378,76 +1405,134 @@
             block_states=block_states,
             data_tags=data_tags,
         )
         return set_location(node, location, data_tags if data_tags else end_location)
 
 
 @dataclass
-class BracketedKeyValuePairsParser:
-    """Parser for bracketed key-value pairs."""
+class BracketedListParser:
+    """Parser for bracketed list."""
 
-    node_type: Type[AstNode]
-    key_parser: Parser
-    value_parser: Parser
+    element_parser: Parser
 
     def __call__(self, stream: TokenStream) -> AstChildren[AstNode]:
-        pairs: List[AstNode] = []
+        elements: List[AstNode] = []
 
         with stream.syntax(
             bracket=r"\[|\]",
-            equal=r"=",
             comma=r",",
         ):
             stream.expect(("bracket", "["))
 
             for _ in stream.peek_until(("bracket", "]")):
-                key_node = self.key_parser(stream)
-                stream.expect("equal")
-                value_node = self.value_parser(stream)
-
-                entry_node = self.node_type(key=key_node, value=value_node)  # type: ignore
-                entry_node = set_location(entry_node, key_node, value_node)
-                pairs.append(entry_node)
+                elements.append(self.element_parser(stream))
 
                 if not stream.get("comma"):
                     stream.expect(("bracket", "]"))
                     break
 
-        return AstChildren(pairs)
+        return AstChildren(elements)
+
+
+@dataclass
+class KeyValuePairParser:
+    """Parser for bracketed key-value pairs."""
+
+    node_type: Type[AstNode]
+    key_parser: Parser
+    value_parser: Parser
+
+    def __call__(self, stream: TokenStream) -> AstNode:
+        with stream.syntax(equal=r"="):
+            key_node = self.key_parser(stream)
+            stream.expect("equal")
+            value_node = self.value_parser(stream)
+
+            entry_node = self.node_type(key=key_node, value=value_node)  # type: ignore
+            return set_location(entry_node, key_node, value_node)
 
 
 @dataclass
 class ItemParser:
     """Parser for minecraft items."""
 
-    resource_location_parser: Parser
-    components_parser: Parser
+    node_type: Type[Any]
+    identifier_parser: Parser
+    arguments_parser: Parser
     data_tags_parser: Parser
 
-    def __call__(self, stream: TokenStream) -> AstItem:
-        identifier = self.resource_location_parser(stream)
+    def __call__(self, stream: TokenStream) -> AstNode:
+        identifier = self.identifier_parser(stream)
         location = identifier.location
         end_location = identifier.end_location
 
-        if components := self.components_parser(stream):
+        if arguments := self.arguments_parser(stream):
             end_location = stream.current.end_location
         else:
-            components = AstChildren[AstItemComponent]()
+            arguments = AstChildren[AstNode]()
 
         data_tags = self.data_tags_parser(stream)
 
-        node = AstItem(
+        node = self.node_type(
             identifier=identifier,
-            components=components,
+            arguments=arguments,
             data_tags=data_tags,
         )
         return set_location(node, location, data_tags if data_tags else end_location)
 
 
 @dataclass
+class ItemPredicateAlternativesParser:
+    """Parser for item predicate alternatives."""
+
+    key_parser: Parser
+    value_parser: Parser
+
+    def __call__(self, stream: TokenStream) -> AstItemPredicateAlternatives:
+        alternatives: List[
+            Union[AstItemPredicateTestComponent, AstItemPredicateTestPredicate]
+        ] = []
+
+        with stream.syntax(
+            pipe=r"\|",
+            equal=r"=",
+            tilde=r"~",
+            exclamation=r"!",
+        ):
+            while True:
+                exclamation = stream.get("exclamation")
+                key_node = self.key_parser(stream)
+
+                if stream.get("tilde"):
+                    test_node = AstItemPredicateTestPredicate(
+                        inverted=exclamation is not None,
+                        key=key_node,
+                        value=self.value_parser(stream),
+                    )
+                else:
+                    test_node = AstItemPredicateTestComponent(
+                        inverted=exclamation is not None,
+                        key=key_node,
+                        value=(
+                            self.value_parser(stream) if stream.get("equal") else None
+                        ),
+                    )
+
+                alternatives.append(
+                    set_location(test_node, exclamation or key_node, test_node.value)
+                )
+
+                if not stream.get("pipe"):
+                    break
+
+        node = AstItemPredicateAlternatives(alternatives=AstChildren(alternatives))
+        return set_location(node, alternatives[0], alternatives[-1])
+
+
+@dataclass
 class NoDataTagsConstraint:
     """Constraint that disallows data tags."""
 
     parser: Parser
 
     def __call__(self, stream: TokenStream) -> Any:
         if isinstance(node := self.parser(stream), AstBlock):
@@ -1948,27 +2033,42 @@
 
             close_bracket = stream.expect(("bracket", "]"))
 
             subscript_node = AstNbtPathSubscript(index=index)
             yield set_location(subscript_node, bracket, close_bracket)
 
 
-def parse_particle(stream: TokenStream) -> AstParticle:
-    """Parse particle."""
-    parameters = None
-
-    if isinstance(name := delegate("resource_location", stream), AstResourceLocation):
-        try:
-            parameters = delegate(f"particle:{name.get_canonical_value()}", stream)
-        except UnrecognizedParser as exc:
-            if not exc.parser.startswith("particle:"):
-                raise
+@dataclass
+class ParticleParser:
+    resource_location_parser: Parser
+    generic_parameters_parser: Parser
+
+    def __call__(self, stream: TokenStream) -> AstParticle:
+        """Parse particle."""
+        parameters = None
+
+        if isinstance(
+            name := self.resource_location_parser(stream), AstResourceLocation
+        ):
+            with stream.syntax(hint=r"\{"), stream.intercept("whitespace"):
+                token = stream.peek()
+
+            if token and token.match("hint"):
+                parameters = self.generic_parameters_parser(stream)
+            else:
+                try:
+                    parameters = delegate(
+                        f"particle:{name.get_canonical_value()}", stream
+                    )
+                except UnrecognizedParser as exc:
+                    if not exc.parser.startswith("particle:"):
+                        raise
 
-    node = AstParticle(name=name, parameters=parameters)
-    return set_location(node, name, parameters if parameters else name)
+        node = AstParticle(name=name, parameters=parameters)
+        return set_location(node, name, parameters if parameters else name)
 
 
 def parse_macro_line(stream: TokenStream) -> AstMacroLine:
     """Parse macro line."""
     with stream.syntax(macro_line=r"\$"):
         token = stream.expect("macro_line")
```

### Comparing `mecha-0.92.0/mecha/preprocess.py` & `mecha-0.93.0/mecha/preprocess.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/prototype.py` & `mecha-0.93.0/mecha/prototype.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/1_16.json` & `mecha-0.93.0/mecha/resources/1_16.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/1_17.json` & `mecha-0.93.0/mecha/resources/1_17.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/1_18.json` & `mecha-0.93.0/mecha/resources/1_18.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/1_19.json` & `mecha-0.93.0/mecha/resources/1_19.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/1_20.json` & `mecha-0.93.0/mecha/resources/1_20.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/nesting.json` & `mecha-0.93.0/mecha/resources/nesting.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/resources/patches.json` & `mecha-0.93.0/mecha/resources/patches.json`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/serialize.py` & `mecha-0.93.0/mecha/serialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,41 @@
     "FormattingOptions",
 ]
 
 
 import json
 import re
 from dataclasses import dataclass, field
-from typing import Any, Iterable, Iterator, List, Literal
+from typing import Any, Iterable, Iterator, List, Literal, Union
 
 from beet.core.utils import required_field
 from pydantic.v1 import BaseModel
 
 from .ast import (
     AstBlock,
     AstBlockState,
     AstBool,
     AstChildren,
     AstCommand,
     AstCoordinate,
-    AstItem,
     AstItemComponent,
+    AstItemPredicate,
+    AstItemPredicateAlternatives,
+    AstItemPredicateTestComponent,
+    AstItemPredicateTestPredicate,
+    AstItemStack,
     AstJson,
     AstLiteral,
     AstMacroLine,
     AstMacroLineText,
     AstMacroLineVariable,
     AstMessage,
     AstNbt,
     AstNbtBool,
+    AstNbtCompound,
     AstNbtPath,
     AstNbtPathKey,
     AstNbtPathSubscript,
     AstNode,
     AstNumber,
     AstParticle,
     AstParticleParameters,
@@ -134,15 +139,14 @@
     @rule(AstNode)
     def unserializable(self, node: AstNode, result: List[str]):
         raise ValueError(f"Couldn't serialize {type(node)!r} node.")
 
     @rule(AstVector2)
     @rule(AstVector3)
     @rule(AstParticleParameters)
-    @rule(AstParticle)
     def aggregate(self, node: AstNode, result: List[str]):
         sep = ""
         for child in node:
             result.append(sep)
             sep = " "
             yield child
 
@@ -253,22 +257,50 @@
         yield node.identifier
         if node.block_states:
             yield from self.collection(node.block_states, "[]", result)
         if node.data_tags:
             yield node.data_tags
 
     @rule(AstItemComponent)
-    def item_component(self, node: AstItem, result: List[str]):
+    def item_component(self, node: AstItemComponent, result: List[str]):
         yield from self.key_value(node, "=", result)
 
-    @rule(AstItem)
-    def item(self, node: AstItem, result: List[str]):
+    @rule(AstItemPredicateTestComponent)
+    @rule(AstItemPredicateTestPredicate)
+    def item_test(
+        self,
+        node: Union[AstItemPredicateTestComponent, AstItemPredicateTestPredicate],
+        result: List[str],
+    ):
+        if node.inverted:
+            result.append("!")
+
+        yield node.key
+
+        if node.value:
+            result.append(
+                "~" if isinstance(node, AstItemPredicateTestPredicate) else "="
+            )
+            yield node.value
+
+    @rule(AstItemPredicateAlternatives)
+    def item_alternatives(self, node: AstItemPredicateAlternatives, result: List[str]):
+        pipe = "|" if self.formatting.cmd_compact else " | "
+        sep = ""
+        for test_node in node.alternatives:
+            result.append(sep)
+            sep = pipe
+            yield test_node
+
+    @rule(AstItemStack)
+    @rule(AstItemPredicate)
+    def item(self, node: Union[AstItemStack, AstItemPredicate], result: List[str]):
         yield node.identifier
-        if node.components:
-            yield from self.collection(node.components, "[]", result)
+        if node.arguments:
+            yield from self.collection(node.arguments, "[]", result)
         if node.data_tags:
             yield node.data_tags
 
     @rule(AstRange)
     def range(self, node: AstRange, result: List[str]):
         if node.exact:
             result.append(number_to_string(node.value))
@@ -353,14 +385,22 @@
         sep = ""
         for component in node.components:
             if isinstance(component, AstNbtPathKey):
                 result.append(sep)
             sep = "."
             yield component
 
+    @rule(AstParticle)
+    def particle(self, node: AstParticle, result: List[str]):
+        yield node.name
+        if node.parameters:
+            if not isinstance(node.parameters, AstNbtCompound):
+                result.append(" ")
+            yield node.parameters
+
     @rule(AstMacroLine)
     def macro_line(self, node: AstMacroLine, result: List[str]):
         result.append("$")
         yield from node.arguments
 
     @rule(AstMacroLineText)
     def macro_line_text(self, node: AstMacroLineText, result: List[str]):
```

### Comparing `mecha-0.92.0/mecha/spec.py` & `mecha-0.93.0/mecha/spec.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/mecha/utils.py` & `mecha-0.93.0/mecha/utils.py`

 * *Files identical despite different names*

### Comparing `mecha-0.92.0/pyproject.toml` & `mecha-0.93.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecha"
-version = "0.92.0"
+version = "0.93.0"
 description = "A powerful Minecraft command library"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/mecha"
 repository = "https://github.com/mcbeet/mecha"
 documentation = "https://github.com/mcbeet/mecha"
```

### Comparing `mecha-0.92.0/PKG-INFO` & `mecha-0.93.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecha
-Version: 0.92.0
+Version: 0.93.0
 Summary: A powerful Minecraft command library
 Home-page: https://github.com/mcbeet/mecha
 License: MIT
 Keywords: beet,minecraft,datapack,minecraft-commands,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.10,<4.0
```

