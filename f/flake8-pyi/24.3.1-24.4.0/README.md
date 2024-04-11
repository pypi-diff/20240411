# Comparing `tmp/flake8_pyi-24.3.1.tar.gz` & `tmp/flake8_pyi-24.4.0.tar.gz`

## Comparing `flake8_pyi-24.3.1.tar` & `flake8_pyi-24.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.editorconfig
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.flake8
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20255 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/ERRORCODES.md
--rw-r--r--   0        0        0    92088 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/pyi.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/scripts/typeshed_primer_download_errors.js
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/scripts/typeshed_primer_post_comment.js
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/workflows/check.yml
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/workflows/typeshed_primer.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.github/workflows/typeshed_primer_comment.yml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/F822.pyi
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/aliases.pyi
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/attribute_annotations.pyi
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/calls.pyi
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/classdefs.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/comparisons.pyi
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/defaults.pyi
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/del.pyi
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/disabled_by_default.pyi
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/emptyclasses.pyi
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/emptyfunctions.pyi
--rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/exit_methods.pyi
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/forward_refs.pyi
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/forward_refs_annassign.pyi
--rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/imports.pyi
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/incomplete.pyi
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/literals.pyi
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/names_requiring_values.pyi
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/never_vs_noreturn.pyi
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/pep570.pyi
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/pep604_union_types.pyi
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/pep646_py311.pyi
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/pep695_py312.pyi
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/quotes.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/single_element_tuples.pyi
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/sysplatform.pyi
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/sysversioninfo.pyi
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/test_pyi_files.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/type_comments.pyi
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/typevar.pyi
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/union_duplicates.pyi
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/unused_things.pyi
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/tests/vanilla_flake8_not_clean_forward_refs.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/LICENSE
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/pyproject.toml
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 flake8_pyi-24.3.1/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.editorconfig
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.flake8
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20399 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/ERRORCODES.md
+-rw-r--r--   0        0        0    92123 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/pyi.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/scripts/typeshed_primer_download_errors.js
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/scripts/typeshed_primer_post_comment.js
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/check.yml
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/typeshed_primer.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/typeshed_primer_comment.yml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/F822.pyi
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/aliases.pyi
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/attribute_annotations.pyi
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/calls.pyi
+-rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/classdefs.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/comparisons.pyi
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/defaults.pyi
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/del.pyi
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/disabled_by_default.pyi
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/emptyclasses.pyi
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/emptyfunctions.pyi
+-rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/exit_methods.pyi
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/forward_refs.pyi
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/forward_refs_annassign.pyi
+-rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/imports.pyi
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/incomplete.pyi
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/literals.pyi
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/names_requiring_values.pyi
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/never_vs_noreturn.pyi
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep570.pyi
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep604_union_types.pyi
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep646_py311.pyi
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep695_py312.pyi
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/quotes.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/single_element_tuples.pyi
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/sysplatform.pyi
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/sysversioninfo.pyi
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/test_pyi_files.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/type_comments.pyi
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/typevar.pyi
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/union_duplicates.pyi
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/unused_things.pyi
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/vanilla_flake8_not_clean_forward_refs.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/LICENSE
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/README.md
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/PKG-INFO
```

### Comparing `flake8_pyi-24.3.1/.flake8` & `flake8_pyi-24.4.0/.flake8`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.pre-commit-config.yaml` & `flake8_pyi-24.4.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-toml
       - id: check-merge-conflict
       - id: mixed-line-ending
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.1.1 # must match pyproject.toml
+    rev: 24.3.0 # must match pyproject.toml
     hooks:
       - id: black
         language_version: python3.8
   - repo: https://github.com/pycqa/isort
     rev: 5.13.2 # must match pyproject.toml
     hooks:
       - id: isort
```

### Comparing `flake8_pyi-24.3.1/CHANGELOG.md` & `flake8_pyi-24.4.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## 24.4.0
+
+Bugfixes:
+* Fix Y026 false positive: allow simple assignment to `None` in class scopes
+  if the class is known to be an enum class.
+
 ## 24.3.1
 
 New error codes:
 * Y064: Use simpler syntax to define final literal types.
   For example, use `x: Final = 42` instead of `x: Final[Literal[42]]`
 * Y065: Don't use bare `Incomplete` in parameter and return annotations.
```

### Comparing `flake8_pyi-24.3.1/CONTRIBUTING.md` & `flake8_pyi-24.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/ERRORCODES.md` & `flake8_pyi-24.4.0/ERRORCODES.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/pyi.py` & `flake8_pyi-24.4.0/pyi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1215,15 +1215,15 @@
         (special-cased, because it is so common in a stub),
         and `X = None` (special-cased because it is so special).
         """
         if (
             isinstance(assignment, ast.Subscript)
             or _is_valid_pep_604_union(assignment)
             or _is_Any(assignment)
-            or _is_None(assignment)
+            or (_is_None(assignment) and not self.visiting_enum_class)
         ):
             new_node = ast.AnnAssign(
                 target=target,
                 annotation=ast.Name(id="TypeAlias", ctx=ast.Load()),
                 value=assignment,
                 simple=1,
             )
```

### Comparing `flake8_pyi-24.3.1/.github/scripts/typeshed_primer_download_errors.js` & `flake8_pyi-24.4.0/.github/scripts/typeshed_primer_download_errors.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.github/scripts/typeshed_primer_post_comment.js` & `flake8_pyi-24.4.0/.github/scripts/typeshed_primer_post_comment.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.github/workflows/check.yml` & `flake8_pyi-24.4.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.github/workflows/publish.yml` & `flake8_pyi-24.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.github/workflows/typeshed_primer.yml` & `flake8_pyi-24.4.0/.github/workflows/typeshed_primer.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.github/workflows/typeshed_primer_comment.yml` & `flake8_pyi-24.4.0/.github/workflows/typeshed_primer_comment.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/aliases.pyi` & `flake8_pyi-24.4.0/tests/aliases.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # flags: --extend-ignore=Y037,Y047
 import array
 import builtins
 import collections.abc
+import enum
 import typing
 from collections.abc import Mapping
 from typing import (
     Annotated,
     Any,
     Literal,
     Optional,
@@ -82,7 +83,10 @@
 _PrivateAliasS2: TypeAlias = Annotated[str, "also okay"]
 
 snake_case_alias1: TypeAlias = str | int  # Y042 Type aliases should use the CamelCase naming convention
 _snake_case_alias2: TypeAlias = Literal["whatever"]  # Y042 Type aliases should use the CamelCase naming convention
 
 # check that this edge case doesn't crash the plugin
 _: TypeAlias = str | int
+
+class FooEnum(enum.Enum):
+    BAR = None  # shouldn't emit Y026 because it's an assignment in an enum class
```

### Comparing `flake8_pyi-24.3.1/tests/attribute_annotations.pyi` & `flake8_pyi-24.4.0/tests/attribute_annotations.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/calls.pyi` & `flake8_pyi-24.4.0/tests/calls.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/classdefs.pyi` & `flake8_pyi-24.4.0/tests/classdefs.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/defaults.pyi` & `flake8_pyi-24.4.0/tests/defaults.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/emptyfunctions.pyi` & `flake8_pyi-24.4.0/tests/emptyfunctions.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/exit_methods.pyi` & `flake8_pyi-24.4.0/tests/exit_methods.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/forward_refs.pyi` & `flake8_pyi-24.4.0/tests/forward_refs.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/forward_refs_annassign.pyi` & `flake8_pyi-24.4.0/tests/forward_refs_annassign.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/imports.pyi` & `flake8_pyi-24.4.0/tests/imports.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/incomplete.pyi` & `flake8_pyi-24.4.0/tests/incomplete.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/literals.pyi` & `flake8_pyi-24.4.0/tests/literals.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/names_requiring_values.pyi` & `flake8_pyi-24.4.0/tests/names_requiring_values.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/never_vs_noreturn.pyi` & `flake8_pyi-24.4.0/tests/never_vs_noreturn.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/pep570.pyi` & `flake8_pyi-24.4.0/tests/pep570.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/pep604_union_types.pyi` & `flake8_pyi-24.4.0/tests/pep604_union_types.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/pep695_py312.pyi` & `flake8_pyi-24.4.0/tests/pep695_py312.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/quotes.pyi` & `flake8_pyi-24.4.0/tests/quotes.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/single_element_tuples.pyi` & `flake8_pyi-24.4.0/tests/single_element_tuples.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/sysversioninfo.pyi` & `flake8_pyi-24.4.0/tests/sysversioninfo.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/test_pyi_files.py` & `flake8_pyi-24.4.0/tests/test_pyi_files.py`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/type_comments.pyi` & `flake8_pyi-24.4.0/tests/type_comments.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/typevar.pyi` & `flake8_pyi-24.4.0/tests/typevar.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/union_duplicates.pyi` & `flake8_pyi-24.4.0/tests/union_duplicates.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/tests/unused_things.pyi` & `flake8_pyi-24.4.0/tests/unused_things.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/.gitignore` & `flake8_pyi-24.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/LICENSE` & `flake8_pyi-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/README.md` & `flake8_pyi-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.3.1/pyproject.toml` & `flake8_pyi-24.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 "Homepage" = "https://github.com/PyCQA/flake8-pyi"
 "Source" = "https://github.com/PyCQA/flake8-pyi"
 "Bug Tracker" = "https://github.com/PyCQA/flake8-pyi/issues"
 "Changelog" = "https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
-    "black==24.1.1",            # Must match .pre-commit-config.yaml
-    "flake8-bugbear==24.1.17",
+    "black==24.3.0",            # Must match .pre-commit-config.yaml
+    "flake8-bugbear==24.2.6",
     "flake8-noqa==1.4.0",
     "isort==5.13.2",            # Must match .pre-commit-config.yaml
-    "mypy==1.8.0",
+    "mypy==1.9.0",
     "pre-commit-hooks==4.5.0",  # Must match .pre-commit-config.yaml
-    "pytest==8.0.0",
+    "pytest==8.1.1",
     "pytest-xdist==3.5.0",
     "types-pyflakes<4",
 ]
 
 [project.entry-points]
 "flake8.extension" = {Y0 = "pyi:PyiTreeChecker"}
```

### Comparing `flake8_pyi-24.3.1/PKG-INFO` & `flake8_pyi-24.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flake8-pyi
-Version: 24.3.1
+Version: 24.4.0
 Summary: A plugin for flake8 to enable linting .pyi stub files.
 Project-URL: Homepage, https://github.com/PyCQA/flake8-pyi
 Project-URL: Source, https://github.com/PyCQA/flake8-pyi
 Project-URL: Bug Tracker, https://github.com/PyCQA/flake8-pyi/issues
 Project-URL: Changelog, https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md
 Author-email: Łukasz Langa <=lukasz@langa.pl>
 Maintainer: Sebastian Rittau, Akuli, Shantanu
@@ -28,22 +28,22 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Requires-Dist: ast-decompiler<1.0,>=0.7.0; python_version < '3.9'
 Requires-Dist: flake8<8.0.0,>=6.0.0
 Requires-Dist: pyflakes>=2.1.1
 Provides-Extra: dev
-Requires-Dist: black==24.1.1; extra == 'dev'
-Requires-Dist: flake8-bugbear==24.1.17; extra == 'dev'
+Requires-Dist: black==24.3.0; extra == 'dev'
+Requires-Dist: flake8-bugbear==24.2.6; extra == 'dev'
 Requires-Dist: flake8-noqa==1.4.0; extra == 'dev'
 Requires-Dist: isort==5.13.2; extra == 'dev'
-Requires-Dist: mypy==1.8.0; extra == 'dev'
+Requires-Dist: mypy==1.9.0; extra == 'dev'
 Requires-Dist: pre-commit-hooks==4.5.0; extra == 'dev'
 Requires-Dist: pytest-xdist==3.5.0; extra == 'dev'
-Requires-Dist: pytest==8.0.0; extra == 'dev'
+Requires-Dist: pytest==8.1.1; extra == 'dev'
 Requires-Dist: types-pyflakes<4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # flake8-pyi
 
 A plugin for Flake8 that provides specializations for
 [type hinting stub files](https://www.python.org/dev/peps/pep-0484/#stub-files),
```

