# Comparing `tmp/pydantic_strict_partial-0.4.0.tar.gz` & `tmp/pydantic_strict_partial-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_strict_partial-0.4.0.tar", max compression
+gzip compressed data, was "pydantic_strict_partial-0.4.4.tar", max compression
```

## Comparing `pydantic_strict_partial-0.4.0.tar` & `pydantic_strict_partial-0.4.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-04-10 17:16:50.473995 pydantic_strict_partial-0.4.0/LICENSE
--rw-r--r--   0        0        0     2073 2024-04-10 22:01:37.192192 pydantic_strict_partial-0.4.0/README.md
--rw-r--r--   0        0        0     1182 2024-04-10 19:43:13.768360 pydantic_strict_partial-0.4.0/pydantic_strict_partial.py
--rw-r--r--   0        0        0     5175 2024-04-10 22:01:37.192870 pydantic_strict_partial-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 pydantic_strict_partial-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2073 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/README.md
+-rw-r--r--   0        0        0     1182 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/pydantic_strict_partial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/pydantic_strict_partial/py.typed
+-rw-r--r--   0        0        0     5163 2024-04-10 23:48:48.584518 pydantic_strict_partial-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 pydantic_strict_partial-0.4.4/PKG-INFO
```

### Comparing `pydantic_strict_partial-0.4.0/LICENSE` & `pydantic_strict_partial-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_strict_partial-0.4.0/README.md` & `pydantic_strict_partial-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_strict_partial-0.4.0/pydantic_strict_partial.py` & `pydantic_strict_partial-0.4.4/pydantic_strict_partial/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_strict_partial-0.4.0/pyproject.toml` & `pydantic_strict_partial-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-strict-partial"
-version = "0.4.0"
+version = "0.4.4"
 description = "Makes partial Pydantic models without making fields nullable."
 authors = ["Adrian Dankiv <adr-007@ukr.net>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "partial", "fastapi"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Framework :: Pydantic :: 2",
 ]
 packages = [
-    { include = "pydantic_strict_partial.py", from = "." },
+    { include = "pydantic_strict_partial", from = "." },
 ]
 homepage = "https://github.com/ADR-007/pydantic-strict-partial"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.1"
 
@@ -67,17 +67,17 @@
 
 [testenv:lint]
 deps =
     ruff
     mypy
     pytest
 commands =
-    ruff check pydantic_strict_partial.py tests.py
-    ruff format --check pydantic_strict_partial.py tests.py
-    mypy pydantic_strict_partial.py tests.py
+    ruff check pydantic_strict_partial tests.py
+    ruff format --check pydantic_strict_partial tests.py
+    mypy pydantic_strict_partial tests.py
 
 """
 
 
 [tool.semantic_release]
 version_toml = [
     "pyproject.toml:tool.poetry.version",
@@ -115,16 +115,16 @@
 
 [tool.semantic_release.commit_author]
 env = "GIT_COMMIT_AUTHOR"
 default = "semantic-release <semantic-release>"
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test"]
-minor_tags = ["feat", "docs"]
-patch_tags = ["fix", "perf", "build"]
+minor_tags = ["feat"]
+patch_tags = ["fix", "perf", "build", "docs"]
 
 [tool.semantic_release.remote]
 name = "origin"
 type = "github"
 ignore_token_for_push = false
 
 [tool.semantic_release.publish]
```

### Comparing `pydantic_strict_partial-0.4.0/PKG-INFO` & `pydantic_strict_partial-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-strict-partial
-Version: 0.4.0
+Version: 0.4.4
 Summary: Makes partial Pydantic models without making fields nullable.
 Home-page: https://github.com/ADR-007/pydantic-strict-partial
 License: MIT
 Keywords: pydantic,partial,fastapi
 Author: Adrian Dankiv
 Author-email: adr-007@ukr.net
 Requires-Python: >=3.10,<4.0
```

