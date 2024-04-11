# Comparing `tmp/dodata_core-0.2.8.tar.gz` & `tmp/dodata_core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodata_core-0.2.8.tar", last modified: Wed Mar  6 19:39:02 2024, max compression
+gzip compressed data, was "dodata_core-0.2.9.tar", last modified: Thu Apr 11 17:19:02 2024, max compression
```

## Comparing `dodata_core-0.2.8.tar` & `dodata_core-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.543679 dodata_core-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.539679 dodata_core-0.2.8/.changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.539679 dodata_core-0.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.539679 dodata_core-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-06 19:38:49.000000 dodata_core-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-06 19:38:49.000000 dodata_core-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-06 19:38:49.000000 dodata_core-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-06 19:38:49.000000 dodata_core-0.2.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-06 19:39:02.543679 dodata_core-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-06 19:38:49.000000 dodata_core-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.539679 dodata_core-0.2.8/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1726 2024-03-06 19:38:49.000000 dodata_core-0.2.8/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-06 19:38:49.000000 dodata_core-0.2.8/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-06 19:38:49.000000 dodata_core-0.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 19:38:49.000000 dodata_core-0.2.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-06 19:38:49.000000 dodata_core-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-06 19:38:49.000000 dodata_core-0.2.8/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-06 19:38:49.000000 dodata_core-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 19:39:02.543679 dodata_core-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.535679 dodata_core-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.543679 dodata_core-0.2.8/src/dodata_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-06 19:39:02.000000 dodata_core-0.2.8/src/dodata_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-06 19:39:02.000000 dodata_core-0.2.8/src/dodata_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 19:39:02.000000 dodata_core-0.2.8/src/dodata_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-06 19:39:02.000000 dodata_core-0.2.8/src/dodata_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 19:39:02.000000 dodata_core-0.2.8/src/dodata_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.535679 dodata_core-0.2.8/src/doplaydo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:39:02.543679 dodata_core-0.2.8/src/doplaydo/dodata_core/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-06 19:38:49.000000 dodata_core-0.2.8/src/doplaydo/dodata_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-03-06 19:38:49.000000 dodata_core-0.2.8/src/doplaydo/dodata_core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 19:38:49.000000 dodata_core-0.2.8/src/doplaydo/dodata_core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.565755 dodata_core-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.561755 dodata_core-0.2.9/.changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.561755 dodata_core-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.561755 dodata_core-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-11 17:18:48.000000 dodata_core-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-11 17:18:48.000000 dodata_core-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 17:18:48.000000 dodata_core-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-11 17:18:48.000000 dodata_core-0.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 17:19:02.565755 dodata_core-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 17:18:48.000000 dodata_core-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.561755 dodata_core-0.2.9/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1726 2024-04-11 17:18:48.000000 dodata_core-0.2.9/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-11 17:18:48.000000 dodata_core-0.2.9/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 17:18:48.000000 dodata_core-0.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 17:18:48.000000 dodata_core-0.2.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 17:18:48.000000 dodata_core-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 17:18:48.000000 dodata_core-0.2.9/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 17:18:48.000000 dodata_core-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:19:02.565755 dodata_core-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.557755 dodata_core-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.565755 dodata_core-0.2.9/src/dodata_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 17:19:02.000000 dodata_core-0.2.9/src/dodata_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-11 17:19:02.000000 dodata_core-0.2.9/src/dodata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:19:02.000000 dodata_core-0.2.9/src/dodata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 17:19:02.000000 dodata_core-0.2.9/src/dodata_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 17:19:02.000000 dodata_core-0.2.9/src/dodata_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.557755 dodata_core-0.2.9/src/doplaydo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:02.565755 dodata_core-0.2.9/src/doplaydo/dodata_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 17:18:48.000000 dodata_core-0.2.9/src/doplaydo/dodata_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-04-11 17:18:48.000000 dodata_core-0.2.9/src/doplaydo/dodata_core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:18:48.000000 dodata_core-0.2.9/src/doplaydo/dodata_core/py.typed
```

### Comparing `dodata_core-0.2.8/.github/release-drafter.yml` & `dodata_core-0.2.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/.github/workflows/release-drafter.yml` & `dodata_core-0.2.9/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/.github/workflows/release.yml` & `dodata_core-0.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/.github/workflows/test_code.yml` & `dodata_core-0.2.9/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/.pre-commit-config.yaml` & `dodata_core-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/CHANGELOG.md` & `dodata_core-0.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # CHANGELOG
 
 <!-- towncrier release notes start -->
 
+## [0.2.9](https://github.com/doplaydo/dodata_core/releases/v0.2.9) - 2024-04-11
+
+No significant changes.
+
+
 ## [0.2.8](https://github.com/doplaydo/dodata_core/releases/v0.2.8) - 2024-03-06
 
 No significant changes.
 
 
 ## [0.2.7](https://github.com/doplaydo/dodata_core/releases/v0.2.7) - 2024-02-04
```

### Comparing `dodata_core-0.2.8/LICENSE` & `dodata_core-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/PKG-INFO` & `dodata_core-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodata_core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core for DoData
 Author-email: DoPlayDo <contact@doplaydo.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 DoPlayDo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,14 @@
 Requires-Dist: pytest_regressions; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: maintainer
 Requires-Dist: pylsp-mypy; extra == "maintainer"
 Requires-Dist: python-lsp-server[all]; extra == "maintainer"
 Requires-Dist: python-lsp-ruff; extra == "maintainer"
 
-# DoData Core library 0.2.8
+# DoData Core library 0.2.9
 
 The core defines integral components of the DoData platform.
 
 ## models.py
 
 This module defines the database scheme used by DoData. It contains all SQLModel class definitions.
```

### Comparing `dodata_core-0.2.8/docs/_config.yml` & `dodata_core-0.2.9/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/pyproject.toml` & `dodata_core-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "sqlmodel>=0.0.14"
 ]
 description = "Core for DoData"
 license = {file = "LICENSE"}
 name = "dodata_core"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.2.8"
+version = "0.2.9"
 
 [project.optional-dependencies]
 dev = [
   "ruff",
   "mypy",
   "pre-commit",
   "pytest",
@@ -134,15 +134,15 @@
 src = "src/doplaydo/dodata_core/__init__.py"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.tbump.version]
-current = "0.2.8"  # bump this
+current = "0.2.9"  # bump this
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `dodata_core-0.2.8/src/dodata_core.egg-info/PKG-INFO` & `dodata_core-0.2.9/src/dodata_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodata_core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core for DoData
 Author-email: DoPlayDo <contact@doplaydo.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 DoPlayDo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,14 @@
 Requires-Dist: pytest_regressions; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: maintainer
 Requires-Dist: pylsp-mypy; extra == "maintainer"
 Requires-Dist: python-lsp-server[all]; extra == "maintainer"
 Requires-Dist: python-lsp-ruff; extra == "maintainer"
 
-# DoData Core library 0.2.8
+# DoData Core library 0.2.9
 
 The core defines integral components of the DoData platform.
 
 ## models.py
 
 This module defines the database scheme used by DoData. It contains all SQLModel class definitions.
```

### Comparing `dodata_core-0.2.8/src/dodata_core.egg-info/SOURCES.txt` & `dodata_core-0.2.9/src/dodata_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dodata_core-0.2.8/src/doplaydo/dodata_core/models.py` & `dodata_core-0.2.9/src/doplaydo/dodata_core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     models.py:
         class MyModel(SQLModel):
 
     mymodel.py:
         def special_method(obj):
             ...
 """
+
 from datetime import UTC, datetime
 from enum import StrEnum
 from typing import Optional, TypeAlias, Union
 
 from sqlalchemy import JSON, CheckConstraint
 from sqlalchemy.dialects.postgresql.json import JSONB
 from sqlmodel import Column, Field, Relationship, SQLModel, UniqueConstraint
@@ -31,14 +32,42 @@
 JSON_VARIANT = JSONB().with_variant(JSON(), "sqlite")  # type: ignore[no-untyped-call]
 
 
 def _now() -> datetime:
     return datetime.now(UTC)
 
 
+class Layout(SQLModel, table=True):
+    """A Layout is a class to govern a eda files and accompanying files."""
+
+    __table_args__ = (
+        UniqueConstraint(
+            "layout_id",
+            "version",
+            name="unique_analysis_function_id_version",
+        ),
+    )
+
+    pkey: Optional[int] = Field(default=None, primary_key=True)
+    """Primary key (unique identifier) for a layout."""
+    layout_id: str = Field(index=True)
+    """The name of the project."""
+    eda_suffix: str = Field(index=True)
+    """Suffix of the eda file."""
+    rdb_suffix: Optional[str] = Field(index=True)
+    """Suffix of the drc result file (report database)."""
+    version: int = Field(index=True)
+    """Version for the layout. Automatically incremented by the server on POST."""
+    description: Optional[str] = None
+    """Additional description of the layout."""
+    attributes: dict = Field(sa_column=Column(JSON_VARIANT), default={})  # type: ignore[type-arg]
+    """Additional info about the layout object."""
+    timestamp: datetime = Field(default_factory=_now, index=True)
+
+
 class Project(SQLModel, table=True):
     pkey: Optional[int] = Field(default=None, primary_key=True)
     """Primary key (unique identifier) for the project."""
     project_id: str = Field(index=True, unique=True)
     """The name of the project."""
     suffix: str = Field(index=True)
     """Filetype extension of the project's EDA file (gds, gds.gz, or oas)."""
```

