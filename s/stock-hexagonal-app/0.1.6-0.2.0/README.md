# Comparing `tmp/stock-hexagonal-app-0.1.6.tar.gz` & `tmp/stock-hexagonal-app-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock-hexagonal-app-0.1.6.tar", last modified: Mon Apr  8 06:29:25 2024, max compression
+gzip compressed data, was "stock-hexagonal-app-0.2.0.tar", last modified: Wed Apr 10 08:49:17 2024, max compression
```

## Comparing `stock-hexagonal-app-0.1.6.tar` & `stock-hexagonal-app-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.062400 stock-hexagonal-app-0.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.062400 stock-hexagonal-app-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/.github/workflows/qa.yml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.062400 stock-hexagonal-app-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.062400 stock-hexagonal-app-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.062400 stock-hexagonal-app-0.1.6/src/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/adapters/alpha_vantage_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/src/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/domain/prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/domain/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/src/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/entrypoints/cli_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/helpers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/src/ports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/ports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/src/ports/stock_data_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-08 06:29:25.000000 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 06:29:25.000000 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:29:25.000000 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 06:29:25.000000 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 06:29:25.000000 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 06:29:25.000000 stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:25.066400 stock-hexagonal-app-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:29:07.000000 stock-hexagonal-app-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.203763 stock-hexagonal-app-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/.github/workflows/qa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-10 08:49:17.203763 stock-hexagonal-app-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:49:17.203763 stock-hexagonal-app-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/src/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/adapters/alpha_vantage_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/src/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/domain/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/domain/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/src/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/entrypoints/cli_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/helpers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.199763 stock-hexagonal-app-0.2.0/src/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/src/ports/stock_data_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.203763 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-10 08:49:17.000000 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 08:49:17.000000 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:49:17.000000 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 08:49:17.000000 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 08:49:17.000000 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 08:49:17.000000 stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:49:17.203763 stock-hexagonal-app-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:57.000000 stock-hexagonal-app-0.2.0/tests/__init__.py
```

### Comparing `stock-hexagonal-app-0.1.6/.github/workflows/qa.yml` & `stock-hexagonal-app-0.2.0/.github/workflows/qa.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 name: quality-assurance
 
 on:
   push:
+    tags-ignore:
+      - '**'
+    branches:
+      - '**'
 
 jobs:
   qa:
     runs-on: ubuntu-22.04
 
     steps:
       - uses: actions/checkout@v4
```

### Comparing `stock-hexagonal-app-0.1.6/.github/workflows/release.yml` & `stock-hexagonal-app-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.1.6/.pre-commit-config.yaml` & `stock-hexagonal-app-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.1.6/CONTRIBUTING.md` & `stock-hexagonal-app-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.1.6/LICENSE` & `stock-hexagonal-app-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.1.6/PKG-INFO` & `stock-hexagonal-app-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-hexagonal-app
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python tool for analyzing stock data build on hexagonal architecture.
 Author-email: Jeremiasz Macura <jeremiaszmacura99@gmail.com>
 License: Copyright 2024 Jeremiasz Macura
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -17,24 +17,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typer==0.12.1
+Requires-Dist: pandas==2.2.1
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Provides-Extra: qa
 Requires-Dist: pre-commit==3.7.0; extra == "qa"
 Provides-Extra: upload
 Requires-Dist: build==1.2.1; extra == "upload"
 Requires-Dist: twine==5.0.0; extra == "upload"
 
 # Python CLI tool to analyze stock data
 
+## How to use
+
+```sh
+pip install stock-hexagonal-app
+stock-hexagonal-app --help
+```
+
 ## Hexagonal Architecture
 
 This tool is build using hexagonal architecture with following structure
 
     |--- src/  # package source code
         |--- adapters/  # implementation of the ports defined in the domain
         |--- domain/  # implementation of business logic
```

### Comparing `stock-hexagonal-app-0.1.6/README.md` & `stock-hexagonal-app-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Python CLI tool to analyze stock data
 
+## How to use
+
+```sh
+pip install stock-hexagonal-app
+stock-hexagonal-app --help
+```
+
 ## Hexagonal Architecture
 
 This tool is build using hexagonal architecture with following structure
 
     |--- src/  # package source code
         |--- adapters/  # implementation of the ports defined in the domain
         |--- domain/  # implementation of business logic
```

### Comparing `stock-hexagonal-app-0.1.6/pyproject.toml` & `stock-hexagonal-app-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.1.6"
+version = "0.2.0"
 name = "stock-hexagonal-app"
 authors = [
     {name = "Jeremiasz Macura", email = "jeremiaszmacura99@gmail.com"},
 ]
 description = "Python tool for analyzing stock data build on hexagonal architecture."
 readme = "README.md"
 requires-python = ">=3.11"
@@ -16,14 +16,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "typer==0.12.1",
+    "pandas==2.2.1",
 ]
 
 [project.optional-dependencies]
 docs = [
     "mkdocs==1.5.3",
 ]
 qa = [
@@ -31,15 +32,15 @@
 ]
 upload = [
     "build==1.2.1",
     "twine==5.0.0",
 ]
 
 [project.scripts]
-stock-cli-app = "entrypoints.cli_entrypoint:app"
+stock-hexagonal-app = "entrypoints.cli_entrypoint:app"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project.urls]
 documentation = "https://jeremiaszmacura.github.io/stock-hexagonal-app/"
 source = "https://github.com/Jeremiaszmacura/stock-hexagonal-app"
```

### Comparing `stock-hexagonal-app-0.1.6/src/entrypoints/cli_entrypoint.py` & `stock-hexagonal-app-0.2.0/src/entrypoints/cli_entrypoint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,83 @@
 import logging
 import typer
 from typing_extensions import Annotated
+from enum import Enum
 
 from helpers.logger import logger
+from domain.command_handler import search_for_company_handler
+from adapters.alpha_vantage_adapter import AlphaVantage
+
+
+class AvailableStockDataProviders(str, Enum):
+    alpha_vantage = "alpha_vantage"
 
 
 app = typer.Typer(help="CLI Application for analyzing stock data.")
 
 statistics_app = typer.Typer()
 app.add_typer(statistics_app, name="count-statistics", help="Calculate selected statistics.")
 
 
 @app.command()
 def search_for_company(
     phrase: Annotated[
         str,
         typer.Option(
+            "--phrase",
+            "-p",
             help="Search for company by passed phrase.",
         ),
     ],
-    debug: Annotated[bool, typer.Option("Switch logger debug mode.")] = False,
+    stock_data_provider: Annotated[
+        AvailableStockDataProviders,
+        typer.Option(
+            "--stock-data-provider",
+            "-stp",
+            case_sensitive=False,
+        ),
+    ] = AvailableStockDataProviders.alpha_vantage,
+    debug: Annotated[bool, typer.Option(help="Switch logger debug mode.")] = False,
 ):
     if debug:
         logger.setLevel(logging.DEBUG)
     print(f"Searching for comapny by phrase: {phrase}")
+    if stock_data_provider == AvailableStockDataProviders.alpha_vantage:
+        selected_stock_data_provider = AlphaVantage()
+    search_for_company_handler(selected_stock_data_provider, phrase)
 
 
 @app.command()
 def draw_stock_graph(
     company_symbol: Annotated[
         str,
         typer.Option(
+            "--company-symbol",
+            "-s",
             help="Company stock symbol.",
         ),
     ],
-    debug: Annotated[bool, typer.Option("Switch logger debug mode.")] = False,
+    debug: Annotated[bool, typer.Option(help="Switch logger debug mode.")] = False,
 ):
     if debug:
         logger.setLevel(logging.DEBUG)
     print(f"Drawing stock graph for comapny: {company_symbol}")
 
 
 @statistics_app.command()
 def value_at_risk(
     company_symbol: Annotated[
         str,
         typer.Option(
+            "--company-symbol",
+            "-s",
             help="Company stock symbol.",
         ),
     ],
-    debug: Annotated[bool, typer.Option("Switch logger debug mode.")] = False,
+    debug: Annotated[bool, typer.Option(help="Switch logger debug mode.")] = False,
 ):
     if debug:
         logger.setLevel(logging.DEBUG)
     print(f"Calculating value at risk for: {company_symbol}")
 
 
 if __name__ == "__main__":
```

### Comparing `stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/PKG-INFO` & `stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-hexagonal-app
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python tool for analyzing stock data build on hexagonal architecture.
 Author-email: Jeremiasz Macura <jeremiaszmacura99@gmail.com>
 License: Copyright 2024 Jeremiasz Macura
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -17,24 +17,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typer==0.12.1
+Requires-Dist: pandas==2.2.1
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Provides-Extra: qa
 Requires-Dist: pre-commit==3.7.0; extra == "qa"
 Provides-Extra: upload
 Requires-Dist: build==1.2.1; extra == "upload"
 Requires-Dist: twine==5.0.0; extra == "upload"
 
 # Python CLI tool to analyze stock data
 
+## How to use
+
+```sh
+pip install stock-hexagonal-app
+stock-hexagonal-app --help
+```
+
 ## Hexagonal Architecture
 
 This tool is build using hexagonal architecture with following structure
 
     |--- src/  # package source code
         |--- adapters/  # implementation of the ports defined in the domain
         |--- domain/  # implementation of business logic
```

### Comparing `stock-hexagonal-app-0.1.6/src/stock_hexagonal_app.egg-info/SOURCES.txt` & `stock-hexagonal-app-0.2.0/src/stock_hexagonal_app.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 .github/workflows/qa.yml
 .github/workflows/release.yml
 docs/index.md
 src/__init__.py
 src/adapters/__init__.py
 src/adapters/alpha_vantage_adapter.py
 src/domain/__init__.py
-src/domain/prepare_data.py
+src/domain/command_handler.py
 src/domain/statistics.py
 src/entrypoints/__init__.py
 src/entrypoints/cli_entrypoint.py
 src/helpers/__init__.py
 src/helpers/logger.py
 src/ports/__init__.py
 src/ports/stock_data_provider.py
```

